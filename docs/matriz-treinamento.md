# Matriz de Treinamento

> Módulo de compliance/treinamento: garante que cada colaborador fez os treinamentos que o cargo dele exige, e avisa quando vence.

## Para que serve
Responde "quem precisa fazer o quê, está em dia, e o que está vencido" — em tempo real, para o time inteiro.

## Conceitos
- **Requisito:** uma exigência de treinamento. Pode exigir uma **Habilidade**, um **Curso**, uma **Capacitação** ou uma **Trilha**. Tem opções de **obrigatoriedade**, **validade** (ex: vale 12 meses) e **lembrete** (ex: avisar 30 dias antes de vencer).
- **Cargo = conjunto de filiais:** o requisito se aplica a quem está nas filiais configuradas. Não existe tabela de "cargo" separada — o cargo é representado pelo conjunto de filiais do colaborador. Se a pessoa está naquelas filiais, o requisito vale para ela (automático, sem matrícula manual).
- **Status de cada exigência:** em dia, pendente, em andamento, vencendo, vencido.

## Telas / visões
- **Matriz (pessoa × requisito):** tabela cruzando colaboradores e requisitos, cada célula com cor de status. Visão geral instantânea.
- **Cobertura / Lacunas:** visão gerencial — % de cobertura, quantos em dia, quantos precisam de atenção, quantos vencidos, com filtros (busca, tipo, nível de cobertura).
- **Drill-down:** clicar no colaborador mostra todos os requisitos dele com status, datas de início e conclusão por curso; clicar no requisito mostra todos que precisam cumprir.
- **Cursos obrigatórios para o aluno:** na página de cursos, selo "Obrigatório" e filtro para ver só os obrigatórios.

## Prontidão de turmas
Verifica se os cursos que cumprem um requisito têm **turma** criada (sem turma, o aluno não consegue fazer o curso). Por requisito mostra um placar:
- **Verde:** tudo pronto.
- **Amarelo:** parcial (X de Y pendentes).
- **Vermelho:** nada pronto.

Ao abrir, lista os cursos **agrupados por habilidade**: os que têm turma mostram início/fim; os que faltam têm botão "Criar turma" (cria com um clique, reaproveitando a criação de turma normal da plataforma). Também verifica se o curso está **publicado e não arquivado** — curso arquivado ou não publicado não conta como pronto e não permite criar turma.

## Regra de negócio importante
A aplicação do requisito é **automática por filial**: ao acessar, o sistema verifica os requisitos das filiais do colaborador e mostra. Não há "matrícula" no requisito — pertencer à filial já basta.

---
*Última revisão: jun/2026. Módulo construído sobre o LMS existente (cursos, turmas, capacitações, trilhas).*
