# Relatórios e Analytics

> Catálogo completo dos relatórios da plataforma: o que cada um mostra, filtros, exportação e para quem serve.

## Como a área se organiza
São **dois formatos diferentes**, e é importante não confundir:

| | O que é | Onde fica |
|---|---|---|
| **Dashboards** | Gráficos e tabelas **na tela**, para olhar e filtrar | Itens do **menu "Relatórios"** |
| **Relatórios em Excel** | **Arquivos gerados** sob demanda, para baixar | Dentro do **Painel de Relatórios** |

Além desses:
- **Relatórios contextuais** — abertos de dentro de um curso, capacitação ou turma.
- **Relatórios Rápidos** — relatórios que o próprio usuário cria descrevendo o que quer para a IA.
- **Insights por IA** — análise conversacional, inclusive **em cima de um relatório já gerado**.

> Nota: vários relatórios cruzam os dados pelos **níveis da hierarquia da empresa** (unidade, área, produto, célula — os nomes variam por cliente, pois a hierarquia é configurável). Alguns dashboards indicam na tela que os dados têm **defasagem de consolidação** (tipicamente D+3).

---

## Painel de Relatórios (os relatórios em Excel)
Enquanto o menu entrega **dashboards** (gráficos na tela), o Painel de Relatórios entrega **arquivos em Excel**, gerados sob demanda.

**Como funciona:**
1. Escolhe o relatório no catálogo (com busca, categorias e **favoritos**).
2. Seleciona o **item alvo** quando aplicável (um curso, uma capacitação ou um formulário).
3. Aba **Gerar Período** — define o período e gera.
4. Aba **Histórico** — lista tudo o que já foi gerado, com **download do Excel**; itens ainda em processamento podem ser excluídos.
5. Aba **Agendar** — geração automática recorrente (o relatório chega pronto, sem alguém precisar clicar).
6. **Insight por IA** — cada relatório já gerado tem um botão "**Perguntar à IA sobre este relatório**": abre o chat de insights **com aquele relatório como contexto**, e a IA responde/analisa em cima daqueles dados.

### Catálogo — Cursos *(escolhe-se um curso)*
- **Geral** — desempenho e conclusão dos alunos no curso.
- **Data e Tempo de Realização** — datas de início/fim e tempo gasto por aluno.
- **Avaliação do Curso** — notas e respostas da avaliação de reação.
- **Aderência / % Progresso** — progresso e aderência dos alunos.
- **Envio de Vídeo (Avaliação da Banca)** — vídeos enviados pelos alunos para avaliação.
- **Respostas do Quiz** — respostas dos alunos nos quizzes.
- **Respostas do Quiz (cursos interativos)** — o mesmo, para cursos criados no editor interativo.
- **Respostas da Avaliação (cursos interativos)** — respostas das avaliações finais desses cursos.

### Catálogo — Capacitações *(escolhe-se uma capacitação)*
- **Participantes** — lista e situação de cada participante.
- **Turmas** — turmas da capacitação, com datas e ocupação.

### Catálogo — Gerais *(plataforma inteira)*
- **Geral: cursos por aluno** — consolidado do que cada aluno realizou.
- **Cursos por Aluno** — relatório dedicado do mesmo recorte.
- **Aderência do mês vigente** — consolidado do mês corrente (com agendamento automático).
- **Justificativa de aderência** — justificativas registradas para baixa aderência.
- **Aderência por usuário (supervisores)** — visão de aderência pessoa a pessoa.
- **Aderência por equipe** — aderência agrupada por equipe/grupo.
- **Avaliações** — consolidado das avaliações de reação da plataforma.
- **Tentativas de avaliação (cursos interativos)** — tentativas feitas em cada avaliação.
- **Capacitações — listagem** — todas as capacitações cadastradas.
- **Cursos por capacitação** — quais cursos compõem cada capacitação.
- **Capacitações — turmas** — todas as turmas de todas as capacitações.
- **Capacitações — participantes** — todos os participantes de todas as capacitações.
- **Turmas de trilhas** — turmas das trilhas de aprendizagem.
- **Usuários** — listagem completa, com hierarquia e status.
- **Hierarquias** — a estrutura de filiais/áreas da empresa.
- **Pontos** — pontuação acumulada por usuário (gamificação).
- **Performance de instrutores** — indicadores de desempenho.
- **Listagem de instrutores** — instrutores cadastrados.
- **Cursos por instrutor** — o que cada instrutor ministrou.
- **Instrutores — troca de filial** — solicitações de troca.
- **Acessos por dia e hierarquia** — acessos diários por área.
- **Acessos em páginas** — quais páginas foram acessadas.
- **Lista de presença** — presença registrada.

### Catálogo — Questionários *(escolhe-se um formulário)*
- **Avaliação de Reação** — respostas da avaliação de reação.
- **Avaliação de Ferramenta** — respostas da avaliação de ferramenta.
- **Pesquisa** — respostas de pesquisas.

> A versão anterior do painel era só uma grade fixa com 7 tipos (Geral de Cursos, Notas, Aderência, Avaliações, Turmas, Participantes, Cursos por Aluno).

## Insights por IA (assistente analítico)
Existe em dois lugares:
- **No painel, como item próprio ("Insights (IA)")** — chat livre sobre os dados da plataforma.
- **Em cada relatório gerado** — botão que abre o chat **já com aquele relatório como contexto**.

- **Mostra:** resposta em texto + **visualização automática** (tabela, barras, linha, rosca ou KPI), a consulta usada para chegar ao número, e sugestões de perguntas iniciais.
- **Exporta:** CSV dos dados e PNG do gráfico.
- **Extras:** feedback 👍/👎 na resposta, cópia e histórico de conversas.
- **Serve para:** interpretar o relatório sem abrir o Excel — pergunta em português, recebe a análise e o gráfico.

## Relatórios Rápidos
- **Mostra:** grade de relatórios **criados pelo próprio usuário via IA** (ele descreve o que quer, ex: "aderência por unidade", e a IA monta um relatório parametrizável e reutilizável). Ao abrir, escolhe o período e gera; o resultado vem em tabela, barras, rosca ou insights.
- **Filtros:** categorias (favoritos, meus relatórios, customizadas), busca por título, período.
- **Exporta:** Excel (tabela), PNG (gráfico), CSV (dados da IA).
- **Serve para:** criar relatório sob medida sem pedir desenvolvimento.

---

## Aderência (conformidade com treinamentos)
Família de dashboards que responde "quem deveria fazer, quem fez".

### Aderência (principal)
- **Mostra:** cards de ranking, gráfico de aderência no período, gráfico de cursos realizados por dia do mês e tabela de cursos com barra de progresso. Permite registrar **justificativas** de não-aderência.
- **Filtros:** mês, hierarquia (unidade/área), tipo de turma (mês vigente / reabertos / todos), cursos.
- **Exporta:** Excel (requer permissão de exportação).
- **Serve para:** acompanhamento operacional mensal da conformidade.
> Existe também uma versão anterior (clássica) do mesmo dashboard, com gráficos por hierarquia e rosca de aderência.

### Aderência por curso ("Cursos Reabertos")
- **Mostra:** tabela granular comparando **mês anterior × mês selecionado** por curso e turma, com finalizados e % de aderência, **colorida por faixa** (verde ≥90%, amarelo 70–89%, vermelho <70%). Tem ação para **recriar turmas** dos cursos abaixo de 90%.
- **Filtros:** mês, estratégia (novos / reabertos), filtros por coluna (curso, turma, níveis da hierarquia) e ordenação.
- **Serve para:** achar o curso específico que está puxando a aderência pra baixo — e agir (recriar turma) na hora.

### Aderência — Turma aberta / Turma fechada
- **Mostra:** dois dashboards gêmeos (cards de ranking, gráfico de aderência, cursos por dia, tabela de cursos), cada um isolando um tipo de turma. A versão "fechada" ainda filtra por **classificação** da turma.
- **Filtros:** mês, hierarquia, cursos (+ classificação, na fechada).
- **Serve para:** analisar separadamente turmas abertas e fechadas, que têm dinâmicas diferentes.

### Aderência — Capacitação
- **Mostra:** cards de visão geral de participantes e gráficos de aderência do treinamento escolhido.
- **Filtros:** ano, mês, hierarquia, categorias de treinamento, treinamento específico.
- **Serve para:** aderência detalhada de uma capacitação.

### Aderência — Cap/Andamento
- **Mostra:** cards de visão geral (turmas e participantes) e gráfico horizontal de aderência por turma.
- **Filtros:** ano, mês, hierarquia, modalidade e treinamento.
- **Serve para:** acompanhar capacitações **em andamento** (não concluídas).

### Aderência — Gestor
- **Mostra:** cards (total de alunos, nota média, aderência média), ranking, gráfico e **tabela de alunos** (nome, o que deveria fazer, o que fez, % de aderência, nota), com busca e paginação.
- **Filtros:** **gestor** (obrigatório — sem escolher, a tela fica vazia), mês, hierarquia, cursos.
- **Serve para:** cada gestor acompanhar o próprio time, aluno a aluno.

### Aderência — Gerencial
- **Mostra:** cards de ranking (formação inicial e continuada) e gráficos de distribuição temporal (por dia da semana e por período do dia).
- **Filtros:** período (de/até).
- **Serve para:** leitura executiva de **quando** os treinamentos acontecem.

---

## Gerencial
- **Gerencial (inicial)** e **Gerencial continuada** — tabelas consolidadas por ano/mês, cada uma para o seu programa. Filtros: ano e mês.
- **Gerencial (novo)** — versão integrada: cards de ranking de continuada e inicial lado a lado, gráfico de aderência, tabela de cursos (curso, carga horária, alunos treinados, % de progresso) e tabela de carga horária por hierarquia. Filtros: mês e hierarquia.
- **Serve para:** visão consolidada de diretoria — inicial + continuada num lugar só.

## Carga Horária
- **Mostra:** tabela por mês e por níveis da hierarquia, com número de usuários, cursos (abre detalhe), **barra de aderência** e a **carga horária** destacada por cor. Ordenável por coluna.
- **Filtros:** mês (múltiplo), hierarquia, tipo de turma.
- **Exporta:** sim.
- **Serve para:** medir o investimento de horas de treinamento por área.

## Trilhas
- **Mostra:** cards de resumo e gráficos por trilha, com opção de ver **em andamento** ou **finalizados**.
- **Filtros:** período (de/até), hierarquia, segmento, produto e trilha(s) de destino.
- **Exporta:** Excel.
- **Serve para:** acompanhar progressão nas trilhas de aprendizado.

## Instrutores (Formação Inicial e Continuada)
- **Mostra:** cards de visão geral dos instrutores e **tabela de desempenho** (nome, quantidade de turmas, participantes, aderência, nota média), ordenável, com detalhe das turmas/cursos de cada instrutor.
- **Filtros:** ano, mês, hierarquia (e, na continuada, também status ativo/inativo e mês múltiplo).
- **Serve para:** avaliar a performance de quem ministra os treinamentos.

---

## Central de Dúvidas (QA)

### Dashboard
- **Mostra:** cards (total de perguntas, % respondidas, % sem resposta, % de baixa relevância, tópicos frequentes), gráfico de perguntas por dia, rosca de distribuição por relevância (alta/média/baixa), barras com as **fontes mais consultadas** e o feedback/satisfação dos usuários.
- **Filtros:** período (7/15/30/60/90 dias).
- **Exporta:** Excel/CSV (todas as perguntas, só as não respondidas, ou só as de baixa relevância).
- **Serve para:** ver se a IA está respondendo bem e onde ela falha.

### Detalhe das perguntas
- **Mostra:** lista paginada de perguntas (texto, data, % de relevância), expansível para ver a resposta e as fontes; e uma aba de **tópicos frequentes** (ranking das perguntas repetidas, com contagem).
- **Filtros:** visão (todas / respondidas / sem resposta / baixa relevância / tópicos), período, status da resposta, limiar de relevância e busca por texto.
- **Exporta:** CSV.
- **Serve para:** achar as lacunas da base de conhecimento — o que os alunos perguntam e a IA não responde bem.

---

## Acessos

### Dashboard de acessos
- **Mostra:** cards (total de usuários, online agora, ativos hoje, ativos na semana, média diária, nunca acessaram), gráfico de usuários únicos por dia, distribuição por **dispositivo** (desktop/mobile/tablet) e tabela dos últimos acessos (usuário, grupos, quando, status).
- **Filtros:** período (7 a 90 dias).
- **Serve para:** medir engajamento e uso real da plataforma.

### Mapa de acesso ao vivo
- **Mostra:** total de usuários online **agora** e a distribuição em tempo real por categoria de tela (Cursos, Capacitações, Conteúdo, Trilhas, Navegação, Interação, Avaliações, Gamificação, Administração), com a lista de telas de cada categoria e **quem** está em cada uma.
- **Filtros:** nenhum (é tempo real).
- **Serve para:** enxergar onde as pessoas estão navegando neste momento.

---

## Questionários (Formulários)
- **Mostra:** ranking e um gráfico de barras por pergunta do formulário, com a distribuição das respostas (e média, nas escalas de concordância).
- **Filtros:** período (ano/mês) e filtros dinâmicos conforme o tipo de pergunta.
- **Serve para:** ler o resultado de pesquisas e avaliações de reação.

## Aluno
- **Mostra:** perfil do aluno (foto, status, grupo, hierarquia, último acesso) e a tabela do que ele fez — cursos, capacitações e trilhas — com turma, categorias, status, **progresso %**, nota e data de conclusão.
- **Filtros:** busca do aluno (nome/matrícula) e abas por tipo (cursos/capacitações/trilhas).
- **Exporta:** Excel.
- **Serve para:** ver o histórico completo de um colaborador.

## Relatórios contextuais
Abertos de dentro do item, não pelo menu:
- **De um curso** — hub com os relatórios daquele curso (ex: respostas do quiz).
- **De uma capacitação** — hub com os relatórios daquela capacitação.
- **De uma turma** — relatório de respostas do quiz da turma.
- **Serve para:** o instrutor analisar o próprio conteúdo sem passar pelo painel geral.

## Registro de Logs
Auditoria das ações na plataforma — ver `extras-e-configuracoes.md`.

## Mapa do Conhecimento e Lacunas (Método PAH)
Análise de conhecimento por IA — ver `endoia-recursos.md`.

---

## Filtros e exportação (padrões)
- **Filtros recorrentes:** período (mês/ano ou de–até, com atalhos de 7 a 90 dias), níveis da hierarquia, curso/capacitação/trilha, status e busca por nome.
- **Exportação:** os principais relatórios exportam em **Excel**; a Central de Dúvidas exporta **CSV**; os gráficos da IA exportam **PNG**. Exportar costuma exigir permissão específica.

## Quem usa o quê
- **Admin** — tudo.
- **Gestor** — aderência (do próprio time), gerencial, carga horária, acessos.
- **Instrutor** — relatórios dos seus cursos, turmas e alunos.
- **Aluno** — apenas o próprio desempenho.

---
*Última revisão: jun/2026.*
