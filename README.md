# Endoo — Base de Conhecimento

Documentação **autossuficiente** sobre a plataforma Endoo: o que cada parte faz, como funciona e os números/decisões que importam.

Este repositório contém **apenas conhecimento** — nenhum código-fonte. Foi feito pra ser lido por pessoas e por assistentes de IA (Claude e outros) que **não têm acesso ao código**. Por isso cada documento se explica sozinho: você não precisa abrir nenhum arquivo de código pra entender.

## Como usar
1. Comece pelo índice geral [`modulos-da-plataforma.md`](modulos-da-plataforma.md) — lista TODOS os módulos e leva ao documento de cada um.
2. Abra o documento detalhado (em `docs/`) do tópico que você precisa.

## Como manter atualizado
- Quem tem acesso ao código (e a um assistente que lê o código) destila o conhecimento aqui em prosa.
- Atualizou? **commit + push**. Quem consome dá `git pull` e recebe a versão nova.
- Convenção: um assunto por arquivo, sempre autossuficiente, sempre com os números reais quando existirem.

## O que NÃO vai aqui
- Código-fonte.
- Segredos/credenciais (chaves, tokens, senhas).
- Caminhos de arquivo de código como "substância" — no máximo como migalha opcional no rodapé.
