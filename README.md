# Projeto de Classificação de Flores com Machine Learning

Projeto de Classificação de Flores com Machine Learning

Objetivo
O objetivo deste projeto é construir um modelo de machine learning capaz de classificar flores da base de dados Iris em uma das três espécies: Iris setosa, Iris versicolor, e Iris virginica. A classificação será baseada nas seguintes características: comprimento da sépala, largura da sépala, comprimento da pétala e largura da pétala. Além disso, o modelo deve ser disponibilizado por meio de uma API que permita seu uso por outras aplicações.

Base de Dados
A base de dados utilizada foi obtida na seguinte URL: https://archive.ics.uci.edu/dataset/53/iris Iris Dataset. O conjunto de dados contém 3 classes de 50 instâncias cada, correspondendo a diferentes tipos de planta de íris. As classes são linearmente separáveis entre si.

Atividades Realizadas
Criação de Pipeline em Python

Foi desenvolvida uma pipeline para treinamento e avaliação do modelo de machine learning. A pipeline incluiu as etapas de pré-processamento dos dados, treinamento do modelo e avaliação de desempenho.
Desenvolvimento de API em Python

Foi criada uma API em Python que utilizou o modelo treinado para realizar previsões. A API recebeu os seguintes 4 parâmetros:
Comprimento da sépala
Largura da sépala
Comprimento da pétala
Largura da pétala
A API realizou o processo de feature engineering e retornou o resultado da previsão com base nos parâmetros fornecidos.
Instruções de Uso
Treinamento e Avaliação

Uso do Postman para Testar a API

Abra o Postman.
Crie uma nova requisição.
Selecione o método POST.
No campo de URL, insira: http://127.0.0.1:5000/predict.
Vá para a aba Headers e adicione o cabeçalho:
Content-Type: application/json
Vá para a aba Body e selecione o tipo raw. Insira o seguinte JSON no corpo da requisição:

{
  "sepal_length": 5.1,
  "sepal_width": 3.5,
  "petal_length": 1.4,
  "petal_width": 0.2
}

Clique no botão Send para enviar a requisição.
Verifique a resposta no painel de resposta do Postman, que deve conter a previsão da espécie da flor com base nas características fornecidas.
Verificação da API

A resposta da API deve mostrar a previsão da espécie da flor com base nos parâmetros fornecidos. Verifique o resultado no painel de resposta do Postman.
Com estas instruções, você deve ser capaz de reproduzir a pipeline de treinamento e avaliação do modelo e iniciar a API para realizar previsões usando o Postman.

Foi necessário executar o script Python que continha a pipeline para treinar o modelo com a base de dados Iris e avaliar seu desempenho.
Utilização da API

O servidor da API foi iniciado.
Foi enviada uma requisição HTTP POST para o endpoint da API com os parâmetros necessários.
A previsão da espécie da flor foi recebida com base nas características fornecidas.
Este projeto visou criar um modelo eficiente para a classificação de flores e disponibilizar uma interface fácil de usar para integrar o modelo com outras aplicações.
