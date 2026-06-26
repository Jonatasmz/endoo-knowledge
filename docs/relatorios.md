# Relatórios e Analytics

> Suíte de dashboards e relatórios para acompanhar aprendizado, aderência, desempenho e acessos — com filtros, exportação e análise por IA.

## Visão geral
Os relatórios se dividem em **Relatórios Avançados** (dashboards analíticos detalhados) e **Relatórios Rápidos** (consultas em linguagem natural geradas por IA). Ambos usam dados coletados em tempo real e servem a perfis diferentes (admin, gestor, instrutor, aluno), cada um vendo o escopo a que tem direito.

## Relatórios Avançados (admin/gestor)

### Aderência (conformidade)
Acompanham o cumprimento de treinamentos obrigatórios:
- **Aderência geral** — visão consolidada por período, filial e categoria.
- **Aderência por curso** — quantos concluíram, estão em progresso ou atrasados num curso.
- **Aderência de capacitações** — progresso em trilhas e programas.
- **Aderência gerencial / por gestor** — cada chefe acompanha o próprio time.
- **Aderência por turma (aberta/fechada)** — distingue turmas que ainda recebem inscrição das encerradas.

### Gerencial (estratégico)
- **Gerencial geral** — KPIs macro: colaboradores, cursos ativos, horas de aprendizado, taxa de conclusão.
- **Gerencial de continuada** — desempenho em educação continuada (pós-obrigatório).

### Desempenho e aprendizado
- **Treinamentos** — histórico de treinamentos, participantes, datas, conclusões.
- **Cursos** — inscrições, conclusões, tempo médio.
- **Por classe/turma** — performance no nível da turma.
- **Formação inicial e continuada** — onboarding e programas pós-obrigatórios.
- **Carga horária** — horas de aprendizado por colaborador/período e cumprimento de metas.
- **Trilhas** — desempenho em percursos customizados.

### Central de Dúvidas (QA)
- **Dashboard QA** — total de perguntas, respondidas/não respondidas, relevância (alta/média/baixa), satisfação (feedback positivo/negativo), fontes mais consultadas; com gráficos por período.
- **Detalhe de perguntas** — lista filtrável (respondidas/não, baixa relevância, similaridade com a documentação, busca por texto), com exportação.

### Acessos e atividade
- **Dashboard de acessos** — acessos por dia, dispositivos, usuários únicos, picos; quem está online agora, ativos hoje/semana/mês, e quem nunca acessou.
- **Mapa de acesso ao vivo** — em tempo real, mostra quantos usuários estão em cada área (Cursos, Capacitações, Trilhas, Avaliações, Gamificação, Administração, etc.), com a lista de quem está em cada tela.

### Formulários (NiceForms)
Relatórios sobre os formulários (pesquisas, avaliações de reação) — ver `formularios.md`.

## Relatórios por perfil
- **Professor/Instrutor** — seus cursos, seus alunos (drill-down por aluno) e suas turmas (presença, progresso).
- **Aluno** — o próprio desempenho: cursos, conclusões, notas, tempo dedicado, certificados.

## Relatórios Rápidos (IA)
Um agente de IA interpreta perguntas em português e gera a consulta + visualização:
- **Perguntas livres** — ex: "Taxa de conclusão de cursos em abril?", "Quantas horas cada filial dedicou?".
- **Visualização automática** — tabela, barras, linha, pizza ou texto explicativo.
- **Histórico, favoritos e categorias** — refinar consultas anteriores, salvar e reutilizar.
- **Exportação** para Excel.

Fluxo: o usuário pergunta → a IA responde com a visualização → ele refina, salva ou exporta.

## Filtros comuns
Período (com atalhos: semana, mês, customizado), filial/unidade, curso/programa, grupo/departamento, status (não iniciado, em andamento, concluído) e busca por nome.

## Exportação
A maioria dos relatórios exporta em **Excel (.xlsx)**, **CSV** e **PDF**.

## Quem usa
Admins veem tudo; gestores veem o escopo da filial/time; instrutores veem seus cursos/alunos; o aluno vê o próprio desempenho. Cada relatório é protegido por permissão específica.

---
*Última revisão: jun/2026.*
