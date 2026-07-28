# Recursos de Inteligência Artificial (EndoIA)

> Tudo o que a plataforma faz com IA hoje, por recurso: o que é, quem usa e como funciona.

A IA da plataforma roda num serviço próprio que orquestra "agentes" especializados (cada um com um modelo e um propósito). Os recursos abaixo são os que existem e funcionam hoje.

> **Programa de Aquisição de Habilidades** é o nome comercial da suíte de análise de conhecimento por IA. No menu, ele reúne cinco áreas: **Mapa do Conhecimento**, **Lacunas de Conhecimento**, **Área do Aluno** (alunos com maiores lacunas), **Área do Saber** (tópicos/questões mais problemáticos) e **Pílulas** (microlearning de reforço). Cada uma é detalhada abaixo.

## 1. Assistente de criação de cursos
- **Quem usa:** instrutores / criadores de conteúdo.
- **O que faz:** chat conversacional para construir cursos. O usuário adiciona fontes (cursos existentes, textos, PDFs, apresentações), planeja a estrutura de módulos e gera o conteúdo visual automaticamente. Detalhe completo em `criador-de-cursos-ia.md`.

## 2. Central de Dúvidas (QA)
- **Onde:** dentro do player de curso (widget lateral).
- **Quem usa:** alunos durante o curso.
- **O que faz:** o aluno pergunta sobre o curso; a IA busca semanticamente em três fontes (conteúdo do curso, biblioteca e wiki) e gera uma resposta contextualizada. Toda interação é registrada para análise posterior.

## 3. Relatório da Central de Dúvidas
- **Quem usa:** admins / coordenadores.
- **O que faz:** dashboard com todas as perguntas feitas pelos alunos. Identifica tópicos frequentes, filtra por período/status/fonte e exporta os dados. Lê dados já gerados pelo QA — não chama a IA em tempo real.

## 4. Auditoria Didática
- **Onde:** painel do curso → "Auditar Questões com IA".
- **Quem usa:** professores / coordenadores (com permissão).
- **O que faz:** analisa as questões com taxa de erro alta (acima de ~30%). Para cada questão problemática, a IA cruza o enunciado com o conteúdo do curso e gera uma análise explicando por que os alunos erram e sugerindo melhorias.

## 5. Mapa do Conhecimento
- **Quem usa:** admins / coordenadores.
- **O que faz:** agrupa automaticamente todo o conteúdo dos cursos em "temas" por similaridade semântica (clustering). Mostra visualizações (treemap, nuvem de palavras, gráficos) da distribuição do conhecimento por tema, fonte e período. Útil para enxergar onde o conteúdo está concentrado e onde há buracos.

## 6. Lacunas de Conhecimento
- **Quem usa:** admins / coordenadores.
- **O que faz:** cruza os erros dos alunos com o Mapa do Conhecimento. Identifica quais temas concentram mais erros, quais questões são mais problemáticas e em quais cursos. Permite detalhar por tema com a distribuição das respostas.

## 7. Reforço Contínuo (Microlearning)
- **Quem usa:** alunos (automático).
- **O que faz:** quando o aluno conclui um curso, o sistema identifica os temas que ele mais errou, busca o conteúdo relevante e gera uma "pílula de revisão" personalizada para reforço.
- **Status:** a geração existe e funciona; a exibição do widget para o aluno pode estar desativada dependendo da configuração.

## 8. Gerador de "O que você irá aprender"
- **Onde:** painel do curso → seção de informações.
- **Quem usa:** professores (em cursos que já têm conteúdo indexado).
- **O que faz:** lê o conteúdo real do curso e gera automaticamente 3 a 5 tópicos descrevendo o que o aluno vai aprender, com ícones.

## 9. Geração de imagens
- **Onde:** dentro do assistente/editor de criação de cursos.
- **Quem usa:** instrutores.
- **O que faz:** gera imagens sob medida para uso nos cursos. Modelo atual: **gpt-image-2** (OpenAI).

## Infraestrutura compartilhada (resumo)
- **Modelos:** OpenAI (GPT para texto, gpt-image-2 para imagem), Gemini e Claude — escolhidos por agente e configuráveis sem nova publicação.
- **Busca semântica:** o conteúdo (cursos, biblioteca, wiki) é transformado em vetores e armazenado para busca por similaridade.
- **Multiempresa:** todo uso é isolado por site/cliente.
- **Registro de uso:** cada chamada de IA grava o custo real, o agente, o modelo e os tokens.

---
*Última revisão: jun/2026. Fonte: documentação interna de funcionalidades de IA.*
