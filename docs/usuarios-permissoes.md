# Usuários, grupos, permissões e filiais

> Como o acesso e a visibilidade são controlados: quem é quem, o que cada um pode fazer e o que cada um enxerga.

## Usuários
Um usuário é um colaborador da plataforma. Tem nome, e-mail, nome de usuário, senha, e **status** (ativo/inativo — desativa sem apagar o histórico). O tipo de autenticação pode ser padrão (usuário/senha), login corporativo (SSO/SAML) ou dupla checagem. Opcionalmente: foto, data de nascimento e um perfil com estatísticas de aprendizagem (cursos feitos, média de notas, pontos).

Cada usuário pertence a **um único site/cliente** (multiempresa) e pode estar vinculado a uma ou mais **filiais**.

## Grupos de permissão
Em vez de permissão individual, usa-se **grupos** — conjuntos nomeados que reúnem funcionalidades. Exemplos típicos: Administrador (acesso total), Instrutor (cria cursos/turmas, vê relatórios), Aluno (faz cursos), RH (gerencia usuários e capacitações), Gestor (vê relatórios do time). Um usuário pode estar em **vários grupos** ao mesmo tempo (as permissões somam).

## Permissões
Uma permissão autoriza uma ação específica (ex: administrar cursos, ver relatórios, gerenciar usuários, exportar dados). As permissões são **hierárquicas**: uma permissão "pai" pode reunir várias filhas. Existem ainda **permissões temporárias** — um admin concede um acesso extra a alguém por um período (ex: até 31/12); ao vencer, cai automaticamente.

Quando o usuário tenta uma ação, a plataforma verifica as camadas (grupo do usuário, configuração do site, permissões temporárias) — autorizando se alguma permitir.

## Filiais (hierarquia organizacional)
A organização é estruturada numa **árvore de filiais** com até **5 níveis** (ex: Regional → Filial → Departamento → Setor → Equipe). Cada nível é tipificável (o admin nomeia as categorias). É essa hierarquia que representa o "cargo/lotação" e governa a visibilidade.

Vincular **usuários** a filiais controla:
- **Visibilidade de conteúdo** — cursos/jornadas de uma filial só aparecem para quem é dela.
- **Relatórios filtrados** — um gestor de filial vê só os dados da filial dele.
- **Inscrições restritas** — o aluno só entra em turmas da sua filial.

Vincular **cursos/turmas/capacitações** a filiais permite treinamentos customizados por região, conformidade local e alocação por divisão. (A Matriz de Treinamento usa exatamente esse conjunto de filiais para decidir o que se aplica a cada pessoa — ver `matriz-treinamento.md`.)

## Login e sessão
O usuário entra com usuário/senha (ou login corporativo). Validado, recebe um token; a plataforma carrega seu grupo, permissões e filiais. Cada requisição seguinte valida o token. As sessões expiram por segurança e exigem novo login.

## Inativação automática
A plataforma pode **inativar automaticamente** usuários que ficam muito tempo sem acessar (ex: 120 dias), com **aviso por e-mail** antes/na inativação. Mantém a base limpa e alinhada ao licenciamento por usuário, sem apagar o histórico (o usuário fica inativo, não excluído). Os critérios são configuráveis conforme o projeto.

---
*Última revisão: jun/2026.*
