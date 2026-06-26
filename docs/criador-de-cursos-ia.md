# Construtor de Cursos com IA + Editor Habilize

> Como nasce um curso no Endoo: do material bruto à publicação, com IA e editor visual. Inclui os modos de exportação (HTML/SCORM).

## Em uma frase
Uma ferramenta de autoria que une **IA** (estrutura e escreve o curso a partir do seu material) e um **editor visual sem código** (você ajusta arrastando e soltando), com mais de 25 atividades interativas, identidade visual da marca, geração de imagens por IA e exportação para qualquer plataforma.

## As três peças
1. **Assistente de IA** — um chat onde o criador junta as fontes (PDFs, apresentações, textos, cursos existentes), pede para planejar a estrutura e gerar o conteúdo.
2. **Motor de geração (IA)** — os agentes que fazem o trabalho: um **planeja os módulos**, outro **gera o conteúdo de cada módulo**, outro **transforma em página visual** (com seções, colunas, imagens, quizzes).
3. **Editor Habilize** — o editor visual onde o curso é montado e refinado. Abre embutido dentro do assistente.

## Fluxo de criação (passo a passo)
1. **Fontes:** o criador anexa o material (PDF, PPT, texto) ou aproveita cursos internos.
2. **Planejar:** a IA propõe uma estrutura de módulos (títulos, descrições, tópicos), editável.
3. **Gerar:** módulo a módulo, a IA escreve o conteúdo (em streaming — o criador vê acontecer).
4. **Montar visual:** o conteúdo vira páginas visuais no editor, com seções, imagens e atividades.
5. **Refinar:** o criador edita à mão ou **pede ajustes em linguagem natural** ("reescreve isso", "troca a imagem", "insere um quiz") e a IA executa.
6. **Publicar/Exportar.**

## Recursos principais
- **Criação automática com IA** a partir de material existente.
- **Editor visual sem código** (arrastar e soltar páginas, seções e atividades).
- **+25 atividades interativas:** quiz, prova, flip-card, jogo da memória, arrastar-e-soltar, preencher lacunas, caça-palavras, ligue os pontos, ordenação, trilha gamificada, carrossel, sanfona, abas, áudio, vídeo, pop-up, tooltip, ebook, e mais.
- **Identidade da marca:** cores, fontes e temas; templates reutilizáveis para padronizar em escala.
- **Geração de imagens por IA** dentro do editor (modelo gpt-image-2 da OpenAI).
- **Assistente de edição** por linguagem natural.
- **Responsivo** por padrão (computador, tablet, celular).

## Exportação e compatibilidade
O curso finalizado pode ser entregue em dois formatos — para uso dentro **ou fora** do Endoo:
- **HTML** — curso autônomo, publicável em qualquer site, intranet ou portal, sem depender de plataforma; abre direto no navegador.
- **SCORM** — pacote no padrão internacional de e-learning, **compatível com qualquer LMS** (Moodle, TOTVS e outros). Carrega uma vez e registra progresso, notas e conclusão automaticamente.

A plataforma também **reproduz** pacotes SCORM (roda o conteúdo e salva o progresso do aluno), além de exportá-los.

---
*Migalha (para quem tem o código): assistente no app principal; agentes e geração no serviço de IA; editor é a aplicação Habilize embutida via iframe. Última revisão: jun/2026.*
