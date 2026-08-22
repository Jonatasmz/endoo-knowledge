# Cursos e LMS

> O núcleo de aprendizagem da plataforma: estrutura de cursos, conteúdos, turmas, avaliações e certificados.

## O que é um curso
Um curso é uma unidade de aprendizagem publicada na plataforma. Cada curso tem:
- **Nome e descrição** para apresentar ao aluno.
- **Tipo** (classificação para organização).
- **Status** — rascunho (em criação) ou publicado (disponível aos alunos).
- **Pontos de gamificação** ganhos ao concluir.
- **Certificado** opcional, emitido ao finalizar.

Um curso pode ter uma prova obrigatória ao final, que o aluno precisa passar para ser aprovado.

## Estrutura de conteúdo
Cada curso é dividido em **capítulos** (ou módulos), em sequência. Dentro de cada capítulo há **tarefas** — as unidades de conteúdo que o aluno consome uma a uma. Tipos de tarefa:
- **Vídeo** (upload, YouTube ou Vimeo)
- **Texto** com formatação rica
- **PDF** para leitura/download
- **Áudio**
- **Imagem**
- **Conteúdo interativo** (SCORM ou curso Habilize)
- **Questionário (quiz)**
- **Avaliação de reação** (feedback do aluno)
- **Recebimento de arquivo** (o aluno envia um trabalho)
- **Presença / check-in** (validação de participação presencial)
- **Videochamada** (aula síncrona)

Uma tarefa pode ter várias seções internas (ex: um vídeo com texto complementar), formando uma hierarquia de conteúdo.

## Turmas e participantes
Um curso é oferecido em **turmas** — grupos de alunos com:
- **Período** (data de início e fim).
- **Limite de vagas**.
- **Filiais** a que se aplica (controla a visibilidade).
- **Situação da turma**, incluindo **Cancelada** — turmas canceladas são desconsideradas nos relatórios e dashboards (não contam na aderência/desempenho).

Um **participante** é um aluno inscrito numa turma. Para cada um, a plataforma registra:
- **Progresso** (0–100%).
- **Status** (em andamento, concluído, reprovado, faltou).
- **Nota final** (se houver prova).
- **Tempo de estudo**.
- **Tarefas concluídas**.

Instrutores podem **importar participantes** em massa por planilha, sem inscrição manual.

## Como o aluno aprende
Ao entrar no curso, o aluno vê os capítulos em ordem; ao abrir um capítulo, consome as tarefas na sequência. Cada tarefa é marcada como concluída (manual ou automaticamente, conforme o tipo).

### Controle de ritmo
- **Tempo mínimo por atividade:** cada tarefa pode exigir um tempo mínimo de permanência. Enquanto ele não é cumprido, aparece uma contagem regressiva e o botão de avançar fica bloqueado — o aluno não pula o conteúdo.
- **Liberação sequencial:** a próxima tarefa só é habilitada quando a anterior é concluída.
- **Configurações de atenção:** o curso pode exibir o cronômetro durante a aula e pausar o vídeo quando o aluno troca de aba.

### O que fica registrado
A plataforma guarda, por aluno:
- **Tempo gasto em cada tarefa.**
- **Cada conteúdo concluído, com data e hora.**
- **Progresso (%) e nota** no curso.
- **Respostas e tentativas** das avaliações.
- **Navegação** (quais páginas acessou e quando).

Esse histórico é mantido ao longo do tempo — não há expurgo automático de registros —, o que permite comprovar a realização do treinamento em auditorias.

## Avaliações e provas
Existe um banco de avaliações — questionários parametrizáveis que podem virar provas obrigatórias do curso. Uma prova tem:
- **Questões de múltipla escolha** (uma alternativa correta), corrigidas automaticamente.
- **Nota mínima** de aprovação, que define aprovado/reprovado.
- **Versões** (ex: prova original e reteste).

Cada tentativa é registrada por aluno, com **as respostas dadas, a nota e a data/hora**. Quem reprova pode refazer conforme o instrutor permitir.

Para avaliação **prática ou situacional**, além da prova objetiva o curso pode usar tarefas de:
- **Envio de arquivo** — o aluno entrega um trabalho.
- **Envio de vídeo para avaliação da banca** — o aluno grava e envia; avaliadores analisam.
- **Atividades dos cursos interativos** — os cursos criados no editor visual têm quizzes e avaliações próprios, com registro de tentativas.

## Certificações
Cursos podem ter um **certificado** (modelo personalizável) emitido em **PDF** quando o aluno conclui com aprovação. O aluno baixa e arquiva o arquivo.

**Campos preenchidos automaticamente no modelo:** nome do aluno, nome do curso, data de conclusão e carga horária.

**Autenticidade e verificação:**
- Cada emissão gera um **código único** de validação.
- O certificado traz um **QR Code** que leva à página de verificação.
- A **verificação é pública** — qualquer pessoa (auditor, empresa contratante) confere a autenticidade **sem precisar de login**, e vê se o certificado é válido, de quem é, de qual curso, a carga horária e a data.
- Os dados ficam **congelados na emissão** (snapshot): mesmo que o curso mude depois, o certificado continua refletindo o que foi cursado.
- O administrador pode **revogar** um certificado; a revogação fica registrada com data e responsável, e a página de verificação passa a mostrar que ele não é mais válido.

## Recursos adicionais
- **Avaliação do curso:** o aluno dá nota em estrelas (1–5) e deixa feedback.
- **Duplicação:** um curso pode ser duplicado com toda a estrutura, para reaproveitar.
- **Reação:** formulários de avaliação de reação podem ser anexados como tarefa (ver `formularios.md`).

---
*Última revisão: jun/2026.*
