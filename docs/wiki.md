# Base de Conhecimento (Wiki)

> Repositório de artigos internos que os colaboradores consultam — e que também alimenta as respostas da IA.

## Para que serve
Documentar processos e políticas, guardar manuais e referências, responder dúvidas frequentes e centralizar o conhecimento da empresa. Os artigos também são indexados para a **Central de Dúvidas** (a IA usa a wiki como uma das fontes de resposta — ver `endoia-recursos.md`).

## Categorias
Os artigos são organizados em **categorias** hierárquicas (categorias e subcategorias), cada uma mostrando quantos artigos contém. Categorias podem ser ativas/inativas e visíveis/ocultas (ocultas só para administradores).

## Artigos
Cada artigo tem título, endereço amigável (slug), conteúdo formatado (editor visual com negrito, listas, imagens e links), categoria, autor, **status** (rascunho ou publicado) e contador de visualizações. Rascunho só aparece para o autor e administradores; publicado, para todos os colaboradores autenticados. A ordem dos artigos dentro de uma categoria pode ser ajustada manualmente. Alterações ficam registradas (quem mudou o quê e quando).

## Buscar e ler
O colaborador navega pelas categorias, busca por palavra-chave (título e conteúdo) ou vê os artigos mais acessados. Ao abrir um artigo, vê o conteúdo formatado, categoria e autor, sugestões de artigos relacionados (mesma categoria) e pode compartilhar o link. Cada leitura incrementa o contador de visualizações.

## Integração com IA
- Os artigos viram representações vetoriais (embeddings) e ficam disponíveis para busca semântica.
- Quando alguém pergunta na Central de Dúvidas, o sistema busca artigos relevantes e os usa como contexto para a IA responder, oferecendo o link do artigo junto.
- Os artigos também entram no **Mapa do Conhecimento** (agrupamento por tema) e na análise de **Lacunas de Conhecimento**.

## Ciclo de vida
Criação (admin escreve e publica) → consulta (colaboradores usam como referência) → atualização (revisão conforme o processo muda) → arquivamento (artigo obsoleto vira inativo, mantido para histórico), tudo auditado.

---
*Última revisão: jun/2026.*
