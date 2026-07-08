# Gamificação, Campanhas e Loja de Prêmios

> Como a plataforma engaja o aluno com pontos, metas e recompensas. Esta área foi **remodelada**: hoje gira em torno de **campanhas** com metas, catálogo de prêmios (inclusive gift cards importados da Incentivale), importação de pontos por planilha, dashboard para o aluno e painel de acompanhamento para o admin.

## Conceitos e vocabulário

- **Campanha** — a unidade central de engajamento. Tem período (data de início e fim), descrição, regulamento e imagens (capa, banner da loja, imagem promocional, fundo). Uma campanha ativa é o que o aluno vê na Lojinha; ao encerrar o período, fica marcada como finalizada. Toda campanha pertence a um único cliente (site) e pode ser segmentada por **filiais**.
- **Prêmio** — item resgatável dentro da campanha. Tem nome, descrição, imagem, **custo em pontos** e quantidade disponível. Pode ser um prêmio tradicional (entregue pela própria empresa) ou um **gift card importado da Incentivale**. Um prêmio com custo zero funciona como voucher já liberado.
- **Pontos** — a moeda de gamificação. O aluno acumula pontos e os gasta resgatando prêmios. Cada ponto é um lançamento individual: 100 pontos = 100 lançamentos. Um ponto pode estar **disponível** (ainda não gasto) ou **debitado** (vinculado a um resgate).
- **Meta** — objetivo de desempenho da campanha (coletivo ou individual), com progresso calculado automaticamente a partir dos pontos, ou preenchido à mão.
- **Resgate** — o pedido de um prêmio pelo aluno. Nasce com um status e evolui até a entrega.
- **Peças vinculadas** — banners, notícias e cursos ligados à campanha, que conectam aprendizado à recompensa e alimentam as métricas de engajamento.

## Pontos: como entram

Pontos chegam à campanha por três caminhos:

1. **Gamificação automática** — ações do aluno na plataforma (concluir cursos, participar de atividades) geram pontos, cada um registrando a ação que o originou.
2. **Lançamento manual** — o admin lança pontos para um usuário específico, informando quantidade, descrição e data (padrão: hoje).
3. **Importação por planilha** — o admin sobe uma planilha (Excel/CSV) com pontos em lote (detalhado abaixo).

Cada lançamento nasce **disponível**. Ao resgatar um prêmio, a plataforma marca a quantidade de pontos correspondente ao custo como **debitada**, associando-a àquele resgate.

### Importação de pontos por planilha (dois passos)

A planilha tem quatro colunas: **matrícula** (nome de usuário), **pontos** (inteiro), **data** e **resultado** (opcional — ex: "85%"). O parsing de data é tolerante: aceita dd/mm/aaaa, aaaa-mm-dd e número serial do Excel.

O fluxo é sempre em dois passos, para o admin conferir antes de gravar:

1. **Validação (preview)** — a plataforma processa a planilha **sem gravar nada** e devolve o que passou e o que não passou. Duas categorias:
   - **Rejeitado** (não será importado): matrícula vazia ou pontos não-numéricos; usuário não encontrado ou inativo; data ausente/impossível.
   - **Aviso** (importa, mas sinaliza para revisão): data no futuro ou anterior a 2015; mais de 30% das matrículas não encontradas; mesma matrícula repetida no mesmo dia (os pontos somam); pontuação muito acima do normal (mais de 4× a mediana da planilha ou acima de 1000); soma do dia acima de 3× a média histórica da campanha; usuário fora das filiais da campanha.
2. **Gravação** — o admin confirma (mesmo com avisos) e a plataforma grava as linhas válidas, criando um lançamento por ponto, com a data da planilha. Ao final informa quantos pontos foram gravados e para quantos usuários.

## Metas da campanha

Metas medem o progresso da campanha. Cada meta tem nome, ícone, um **tipo de métrica**, um **escopo** e, quando baseada em pontos, uma **janela de tempo**.

**Tipo de métrica:**
- **Pontos** — progresso calculado automaticamente a partir dos pontos lançados na campanha.
- **Customizada** — o admin edita o progresso à mão (para objetivos que a plataforma não mede sozinha, ex: "80% de conclusão").

**Escopo:**
- **Coletiva** — soma dos pontos de toda a campanha contra um alvo único. Ex: "atingir 5.000 pontos em julho". Progresso = total acumulado ÷ alvo.
- **Individual** — cada participante tem o mesmo alvo pessoal, e a meta mede **quantas pessoas bateram**. Ex: "cada pessoa acumula 10 pontos". Progresso = quem atingiu ÷ total de participantes elegíveis (exibe também "X de Y bateram").

**Janela de tempo** (para metas de pontos):
- **Diária** — conta só os pontos de hoje (00:00–23:59).
- **Período** — conta os pontos entre uma data de início e fim.
- **Sem janela** — considera todo o histórico.

**Segmentação por filial:** uma meta pode se restringir a filiais específicas. Sem filiais próprias, herda as filiais da campanha; se a campanha também não tem, aplica a todos os usuários ativos do cliente.

O progresso é exibido em barra/velocímetro com percentual (0–100%) e, para metas de período, uma **série diária** para o gráfico de evolução.

## Loja de Prêmios (Lojinha) — o aluno

O aluno acessa a **Lojinha** e vê as campanhas ativas mais um resumo dos próprios prêmios (não resgatados, resgatados, expirados) e o histórico recente de resgates.

Ao abrir uma campanha, encontra quatro abas:
1. **Detalhes** — resumo do próprio desempenho (posição no ranking, pontos do mês, progresso médio das metas) + descrição e imagem promocional.
2. **Regulamento** — o texto de regras da campanha.
3. **Lojinha** — saldo de pontos ("X disponíveis") com link para o extrato, banner da campanha e a grade de prêmios (imagem, nome, custo em pontos, selo "resgatado N×"). Clicar num prêmio abre o detalhe com o botão de resgate.
4. **Meu Desempenho** — visão gamificada do aluno (nível, posição, metas em velocímetro, simulador de "faltam X pontos para o próximo nível", evolução mensal, comparação com a média da equipe). *Parte desta aba ainda é protótipo com dados ilustrativos.*

Há também um **catálogo de produtos** (os itens importados da Incentivale) navegável com filtros por categoria, filial, campanha e "apenas o que cabe no meu saldo", busca por nome, ordenação por preço/relevância e carregamento sob demanda (12 por vez).

**Extrato de pontos:** o aluno abre o extrato e vê o histórico de lançamentos mais um gráfico de pontos por dia.

## Resgate de prêmios

Há dois tipos de resgate, com fluxos diferentes:

### Prêmio tradicional (imediato)
O aluno resgata; a plataforma cria o resgate já como **entregue**, debita os pontos e reduz a quantidade disponível. Se o prêmio tem um código de voucher, ele aparece no resgate do aluno. Prêmios com custo zero são tratados como voucher já liberado.

### Gift card Incentivale (assíncrono)
Ao resgatar um item Incentivale, o aluno confirma **CPF/CNPJ** e **aceita os termos**. A plataforma gera um código de pedido próprio, chama a API da Incentivale e cria o resgate como **pendente**, guardando o código do pedido e o código de transação da Incentivale. Os pontos são debitados na hora. O CPF/CNPJ informado **não é armazenado** — só trafega para a Incentivale no pedido. Depois, o status é acompanhado por consulta ao pedido: quando a Incentivale marca como entregue, o código do gift card fica disponível para o aluno.

O tipo de produto Incentivale define o endpoint usado no pedido: cartão virtual (padrão), crédito em conta, pagamento de contas ou recarga de celular.

**Estados de um resgate:** pendente (aguardando entrega — típico da Incentivale), entregue, expirado.

## Importação de produtos da Incentivale — o admin

Na aba **Lojinha** da campanha, o admin clica em "Importar do Incentivale". A plataforma consulta ao vivo o catálogo da Incentivale (apenas gift cards com preços definidos) e **expande cada produto por suas denominações** — cada valor em reais vira uma linha. O admin marca as linhas desejadas e ajusta o **custo em pontos** (pré-preenchido com o valor em R$).

Ao importar, cada denominação selecionada vira **um prêmio** na campanha, com a origem "incentivale" e seus metadados (SKU, categoria, filial, preço, imagem — a imagem é baixada e anexada). A plataforma ignora itens já importados na campanha e informa quantos entraram e quantos foram pulados.

> Detalhe de contrato: a integração autentica por usuário/senha e reaproveita o token por ~9 minutos (a API expira em 10). Endpoints e credenciais estão documentados fora desta base.

## Painel do Admin

O admin gerencia campanhas em uma lista com status (ativa/finalizada), período e estatísticas de prêmios. Ao criar/editar, tem abas para: **Detalhes** (nome, datas, descrição, imagens), **Regulamento**, **Lojinha** (banner + prêmios, com botões de adicionar prêmio e importar da Incentivale), **Peças** (vincular banners, notícias e cursos), **Metas** (CRUD de metas com progresso) e **Pontos** (lista de participantes com saldo, lançamento manual e importação por planilha).

Há ainda um **painel de acompanhamento** por campanha, com dados reais de: resumo de conteúdo (quantos banners, notícias e cursos vinculados), métricas de engajamento das peças (leituras/curtidas de notícias, cliques em banners, matrículas e conclusões dos cursos vinculados), e as metas com progresso e série diária. Um botão gera um relatório de participantes que pode ser analisado pela IA da plataforma. *Uma seção "protótipo gestor" (heatmap de pontos, correlações, ROI, produtos mais trocados) ainda usa dados ilustrativos.*

## Controle por filial

A segmentação por filial atravessa tudo: campanhas podem se restringir a filiais (sem restrição = abertas a todos), metas herdam ou definem as próprias filiais, e o catálogo permite ao aluno filtrar por filial. Assim cada parte da organização vê as campanhas e prêmios que lhe cabem.

## Resumo do papel

A gamificação estimula a conclusão de treinamentos: o aluno aprende, ganha pontos, acompanha metas e troca por recompensas reais — inclusive gift cards de marcas via Incentivale. As campanhas amarram conteúdo (cursos/notícias/banners), metas e prêmios num período, e o painel do admin fecha o ciclo mostrando engajamento e resultado.

---
*Última revisão: jul/2026.*
