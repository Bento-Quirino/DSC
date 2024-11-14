# Projetos Simples de IA em Python

Este repositório contém 10 projetos simples usando Python e bibliotecas de IA/Machine Learning, ideais para iniciantes. Cada projeto foi pensado para ser executado no Google Colab.

## Projetos

| Projeto | Descrição | Bibliotecas | Instruções de Instalação |
| ------- | --------- | ----------- | ------------------------- |
| 1. Análise de Sentimentos | Analisar a polaridade de sentimentos de textos | `textblob` | `pip install textblob` |
| 2. Detecção de Face em Imagens | Detectar rostos em imagens | `face_recognition`, `opencv-python` | `pip install face_recognition opencv-python` |
| 3. Detecção de Face em Imagens* (ao invés de tensorflow com keras) | Detectar rostos em imagens | `face_recognition`, `opencv-python` | `pip install face_recognition opencv-python` |
| 4. Gerador de Texto com Markov | Gerar frases baseadas em cadeias de Markov | `markovify` | `pip install markovify` |
| 5. Análise de Tópicos | Identificar tópicos principais em textos grandes | `gensim`, `nltk` | `pip install gensim nltk` |
| 6. Classificação de Notícias | Classificar notícias em categorias (ex: política, esportes) | `sklearn` | `pip install scikit-learn` |
| 7. Gerador de Poesias | Criar poesias usando um modelo simples de geração de texto | `torch`, `transformers` | `pip install torch transformers` |
| 8. Tradutor de Idiomas | Traduzir texto entre idiomas | `translate` | `pip install translate` |
| 9. Reconhecimento de Emoções em Texto | Detectar emoções (feliz, triste, etc.) em textos | `text2emotion` | `pip install text2emotion` |
| 10. Resumo Automático de Textos | Criar resumos curtos de textos longos | `sumy` | `pip install sumy` |

## Critérios de Avaliação

Esta tabela apresenta os critérios de avaliação para cada projeto desenvolvido no Google Colab. A pontuação é dada com base na organização, explicação da biblioteca utilizada, descrição do processo de modelagem e clareza do código.

| Critério                        | Descrição                                                                                                        | Pontuação Máxima |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------- |
| **Explicação da Biblioteca**    | Introdução à biblioteca utilizada, com descrição dos principais métodos ou funções.                             | 5 pontos        |
| **Explicação do Processo**      | Descrição clara do que o modelo ou função está realizando (ex: análise de sentimentos ou detecção de faces).    | 2 ponto          |
| **Criação de Função com o modelo(def)**     | O código deve ser modularizado utilizando funções (com `def`). A função principal deve realizar a ação do modelo.(analisar sentimento, comparar rostos, etc) | 3 ponto          |

## Dicas para Estruturar o Colab

1. **Títulos e Seções**: Separe o notebook em seções claras com títulos, como *Introdução*, *Instalação de Bibliotecas*, *Explicação do Processo*, *Código* e *Conclusão*.

2. **Introdução e Explicação**: No início de cada notebook, descreva brevemente o objetivo do projeto e o papel da biblioteca utilizada, explicando como ela funciona (por exemplo, `textblob` para análise de sentimentos ou `face_recognition` para detecção facial).

3. **Processo Explicado em Texto**: Explique o que o processo de modelagem envolve e o que cada célula de código está fazendo, especialmente em blocos de processamento de dados e execução de modelos.

4. **Criação de Funções**: Certifique-se de modularizar o código criando funções com `def`, especialmente para realizar a ação principal do modelo, como "analisar_sentimentos" ou "detectar_faces". As funções ajudam a manter o código organizado e reutilizável.

    **Exemplo**:
    ```python
    def analisar_sentimentos(texto):
        from textblob import TextBlob
        blob = TextBlob(texto)
        return blob.sentiment.polarity
    ```

5. **Comentários no Código**: Adicione comentários no código, especialmente em etapas críticas, como carregamento de dados, execução de funções específicas e interpretação de resultados. Isso torna o código mais fácil de entender e acompanhar.

    **Exemplo**:
    ```python
    # Carregando a imagem e convertendo para escala de cinza
    img = cv2.imread('imagem.jpg')
    gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
    ```

6. **Clareza do Código**: Use nomes de variáveis e funções que sejam intuitivos e representem claramente o que estão fazendo. Isso ajuda a facilitar a compreensão do código por outras pessoas (ou até por você no futuro).

## Instruções para Rodar os Projetos

Cada projeto pode ser aberto em uma célula individual no Google Colab. Lembre-se de instalar as bibliotecas necessárias no ambiente de execução usando `pip install` como indicado acima.
