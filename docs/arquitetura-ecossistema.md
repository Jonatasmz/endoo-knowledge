# Arquitetura do ecossistema Endoo

> Visão geral das partes que compõem o Endoo e como se encaixam. Não é manual técnico — é o mapa pra você saber "o que é cada coisa".

## O que é o Endoo
Plataforma corporativa de educação/treinamento (LMS) com forte camada de **inteligência artificial**, criação de cursos, gamificação e relatórios. Multiempresa: uma mesma instalação atende vários clientes (cada cliente é um "site"/inquilino isolado), e o conteúdo/visibilidade é controlado por **filiais** (a hierarquia organizacional de cada cliente — empresa, área, etc.).

## As partes (repositórios)
- **iendo-front** — Aplicação web principal (o que o usuário final e o admin usam). Cursos, relatórios, gamificação, administração.
- **iendo-api** — Backend principal. Regras de negócio, usuários, cursos, matrículas, turmas, permissões. É o "coração" de dados.
- **iendo-ai** — Serviço de inteligência artificial. Todos os recursos de IA passam por aqui (geração de cursos, perguntas e respostas, mapas de conhecimento, geração de imagem, etc.).
- **iendo-admin** — Painel administrativo de bastidor (criação de sites/clientes, planos, processamento de pagamentos de onboarding).
- **habilize-builder** — Editor visual de cursos (o "construtor"). Aplicação separada, embutida na principal quando se cria/edita um curso.
- **loja-endoo** — Site de vitrine/checkout (marketing + venda de planos/cursos por fora da plataforma).
- **landings** — Páginas de captação.

## Conceitos-chave
- **Site / inquilino:** cada cliente é isolado. Quase tudo é filtrado por site automaticamente.
- **Filiais (hierarquia):** definem quem vê o quê. Um "cargo" pode ser representado por um **conjunto de filiais** (ex: área X da empresa Y). Usado pela Matriz de Treinamento.
- **Curso / Turma:** o curso é o conteúdo; a turma é o agrupamento de alunos com período (início/fim) que torna o curso visível e matriculável para um conjunto de filiais.
- **Participação (matrícula):** o vínculo de um aluno com um curso/capacitação, com status (cursando, aprovado) e progresso.
- **Uso de IA:** cada chamada a um modelo de IA é registrada com o custo real, o agente, o modelo e os tokens usados.

## Camada de IA (resumo)
O serviço de IA orquestra vários "agentes" especializados (planejar curso, gerar módulo, montar página visual, responder dúvidas do aluno, auditar questões, agrupar conhecimento por tema, gerar imagem). Usa modelos da OpenAI (GPT e gpt-image-2 para imagem), Gemini e Claude conforme a tarefa — o modelo de cada agente é configurável sem nova publicação. Detalhe dos recursos de IA em `endoia-recursos.md`.

---
*Última revisão: jun/2026.*
