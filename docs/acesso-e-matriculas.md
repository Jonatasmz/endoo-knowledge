# Acesso, usuários e matrículas

> Como uma pessoa entra na plataforma e como ganha acesso a um curso.

## Usuários
- Cada usuário pertence a um **site** (cliente) e a um conjunto de **filiais** (a hierarquia que define o que ele vê).
- O usuário tem status (ativo/inativo) e credenciais de acesso.
- **Não há auto-cadastro público aberto.** Usuários são criados por um dos caminhos:
  - Criação pelo admin (individual);
  - Importação em massa por planilha (CSV), com **log de importação** (o que entrou e o que falhou);
  - Login único externo (SSO) integrado ao sistema do cliente.
- **Login:** por usuário e senha, com variações (ex: ativar o usuário no primeiro acesso). A sessão é autenticada por token.

## Como o aluno ganha acesso a um curso
Há três mecanismos:

### 1. Turma (o caminho padrão)
- O admin cria uma **turma** do curso, com período (início/fim) e as filiais a que se aplica.
- Os alunos são adicionados como **participantes** da turma (individualmente ou por planilha).
- O aluno passa a ver o curso na lista dele e progride; o status evolui (cursando → aprovado/reprovado), com nota e progresso registrados.
- A turma é o que torna o curso **visível e matriculável** para um conjunto de filiais dentro do período.

### 2. Acesso direto
- O admin concede acesso de um usuário a um curso **diretamente**, sem turma. Útil para liberar um curso pontualmente.

### 3. Campanha
- Uma **campanha** pode ser pública: o próprio usuário se inscreve no curso por conta própria.

## Observações
- Não existe visitante anônimo — para acessar conteúdo é preciso estar autenticado.
- O controle de visibilidade por **filial** atravessa tudo: turmas, campanhas e a Matriz de Treinamento usam o conjunto de filiais do usuário para decidir o que se aplica a ele.

---
*Última revisão: jun/2026.*
