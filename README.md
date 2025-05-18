# 🚀 EduFlow AI: Seu Co-piloto de Aprendizagem Inteligente 🤖

![Capa do Projeto - Seção para adicionar Screenshot/GIF do Colab]
<!-- Adicione aqui um GIF curto ou screenshot da interação no Colab -->

## O Problema: A Aprendizagem Passiva em Cursos Online

No vasto universo dos cursos online (vídeos, áudios, textos), a aprendizagem frequentemente se torna uma experiência passiva. Consumimos conteúdo, mas a ausência de interação pedagógica em tempo real dificulta a fixação do conhecimento, a identificação de lacunas individuais e a prática direcionada. Como garantir que o aluno realmente absorveu e é capaz de aplicar o que aprendeu, além de simplesmente assistir ou ler?

## A Solução: EduFlow AI

O **EduFlow AI** surge como um **co-piloto de aprendizagem inteligente**, projetado para transformar a experiência de estudo online em um processo ativo, interativo e personalizado. Utilizando o poder da **Inteligência Artificial generativa (Google Gemini)**, o EduFlow AI atua como um mentor pedagógico em tempo real, auxiliando o aluno a fixar o conteúdo, identificar pontos de melhoria e praticar de forma direcionada.

Em sua essência, o EduFlow AI opera através de um sistema de agentes especializados, cada um com uma função clara no ciclo de aprendizado e feedback:

*   **Agente de Interação e Boas-Vindas:** O rosto amigável do EduFlow AI. Recebe o aluno, explica o funcionamento, coleta o nome para personalizar a interação e orienta sobre como compartilhar o material de estudo.
*   **Agente de Conteúdo, Avaliação e Feedback:** O cérebro pedagógico. Processa o conteúdo compartilhado pelo aluno, identifica conceitos-chave, gera perguntas de avaliação desafiadoras, recebe e avalia as respostas do aluno, diagnostica lacunas no conhecimento e gera um feedback construtivo e personalizado, incluindo sugestões de reforço.

## Funcionalidades Demonstradas no MVP (Google Colab)

Este repositório apresenta um **MVP (Minimum Viable Product)** do EduFlow AI, implementado como um protótipo funcional no Google Colab. Neste MVP, demonstramos as principais capacidades pedagógicas do sistema:

*   **Interação Inicial e Coleta de Dados:** O EduFlow AI recebe o aluno de forma amigável, coleta o nome e orienta sobre o uso.
*   **Absorção de Conteúdo (Simulada):** O usuário cola manualmente o texto da aula ou tópico de estudo no Colab. O agente de Conteúdo processa este texto para entender o escopo e os conceitos.
*   **Geração de Avaliações:** Com base no conteúdo processado, o agente gera 2-3 perguntas de avaliação que incentivam o pensamento crítico e a aplicação do conhecimento, sem fornecer as respostas diretas. Inclui a capacidade de gerar perguntas que simulam a conexão com "módulos anteriores".
*   **Captura de Respostas:** O sistema captura as respostas do aluno às perguntas geradas via inputs no Colab.
*   **Avaliação e Diagnóstico:** O agente de Conteúdo/Avaliação/Feedback avalia as respostas do aluno em relação ao conteúdo original, determina o acerto/erro (correto, parcialmente correto, incorreto) e diagnostica os conceitos que precisam de reforço.
*   **Feedback Pedagógico e Sugestões de Reforço:** Gera um feedback detalhado, personalizado e motivador, explicando os pontos de acerto/erro e sugerindo tipos de ações para reforçar o aprendizado (revisão, exemplos, prática extra).
*   **Simulação de Conexão entre Módulos:** Através da instrução do agente, simulamos a capacidade de gerar uma pergunta que conecte o conteúdo atual com um tópico "anterior" fornecido pelo usuário.

## Tecnologias Utilizadas

*   **Google Gemini API:** O coração da inteligência do EduFlow AI, utilizado para processamento de linguagem natural, geração de conteúdo (perguntas, feedback) e avaliação.
*   **Google Colab:** Ambiente de desenvolvimento e execução para o protótipo MVP.
*   **Python:** Linguagem de programação utilizada para implementar a lógica dos agentes e o fluxo de execução.
*   **Google ADK (Agent Development Kit):** Framework utilizado para facilitar a criação e gerenciamento dos agentes baseados em modelos de linguagem.

## COMO RODAR O PROJETO (Passo a Passo)

Para experimentar o EduFlow AI no Google Colab, siga estes passos:

1.  **Acesse o Google Colab:** Vá para [colab.research.google.com](https://colab.research.google.com/).
2.  **Abra o Notebook:** Clique em `Arquivo > Fazer upload de notebook` e selecione o arquivo `.ipynb` deste repositório (ex: `eduflow_ai_mvp.ipynb`).
3.  **Configure a API Key do Google Gemini:**
    *   Você precisará de uma API Key do Google Gemini. Se você não tiver uma, pode obtê-la em [aistudio.google.com/access/key](https://aistudio.google.com/access/key).
    *   No Colab, clique no ícone de "chave" (Secrets) no menu lateral esquerdo.
    *   Clique em `+ Novo secret`.
    *   No campo `Nome`, digite `GOOGLE_API_KEY` (exatamente assim).
    *   No campo `Valor`, cole a sua API Key do Google Gemini.
    *   Certifique-se de que a opção `Notebook access` está marcada.
4.  **Rode as Células do Notebook:** Execute cada célula de código sequencialmente, clicando no botão "Play" ao lado de cada célula ou usando atalhos (Shift + Enter).
    *   As primeiras células instalarão as bibliotecas necessárias e configurarão a API Key.
    *   A execução irá pausar para que você interaja via inputs de texto.
5.  **Interaja com o EduFlow AI:**
    *   Siga as instruções que aparecerão no output.
    *   Quando solicitado, digite como você gostaria de ser chamado(a).
    *   Quando solicitado, **cole o texto do material de estudo**. Use um dos exemplos abaixo para testar:

PLANO DE MELHORIAS FUTURA:

Criar uma extensão ou aplicação que ao ser acionado assistira as aulas lado a lado com você e poderá ter mais interações em tempo real sempre sendo seu aliado no aprendizado do conteúdo.
