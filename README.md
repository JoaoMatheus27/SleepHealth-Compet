Classificação de Distúrbios do Sono com Machine Learning

Este projeto foi desenvolvido como parte do **Desafio COMPET – Inteligência Artificial na Prática**. O objetivo é aplicar técnicas de **Aprendizado de Máquina (Machine Learning)** para criar um modelo que detecte distúrbios do sono com base em dados de estilo de vida e saúde.

## Base de Dados

Utilizei o conjunto de dados público [**Sleep Health and Lifestyle Dataset**](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset) disponível no Kaggle. Ele contém informações como:

- Idade
- Gênero
- Frequência cardíaca
- Pressão arterial
- Consumo de café
- Nível de estresse
- Qualidade do sono
- Presença de distúrbios do sono (coluna alvo)

## Etapas Realizadas

## Pré-processamento:
- Remoção de colunas irrelevantes
- Tratamento de valores nulos
- Codificação de variáveis categóricas
- Balanceamento das classes com SMOTE

## Treinamento:
- Divisão dos dados em treino e teste
- Treinamento com dois modelos:
  - **Random Forest**
  - **Regressão Logística**

## Avaliação:
- Avaliação de desempenho com acurácia
- Repetição de 30 execuções para análise de estabilidade (média e desvio padrão)
- Escolha do modelo mais estável e com maior acurácia

## Deploy:
- Salvamento do modelo final com `pickle`
- Criação de uma interface com **Gradio** para uso interativo

## Interface Gráfica (Gradio)

Uma interface interativa foi criada com a biblioteca [Gradio](https://www.gradio.app/) para entrada de dados do usuário e exibição da predição.
