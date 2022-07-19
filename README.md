# Titanic - Machine Learning from Disaster

## Tópicos

:small_blue_diamond: [Descrição do Projeto](#Descrição-do-Projeto)

:small_blue_diamond: [Dicionário de dados](#Dicionário-de-dados)

:small_blue_diamond: [Limpeza e Tratamento de dados](#Limpeza-e-Tratamento-de-dados)

:small_blue_diamond: [Tecnologias utilizadas](#Tecnologias-utilizadas)


# Descrição do Projeto

Este projeto tem por objetivo prever a situação dos passageiros (sobrevivente ou não) diante da tragédia do Titanic. 

# Dicionário de dados

* PassengerId - id do passageiro
* Survived - status Sobrevivente (0 = Não; 1 = Sim)
* Pclass - classe dos passageiros (1 = primeira; 2 = segunda; 3 = terceira)
* Name - nome
* Sex - Sexo
* Age - idade
* SibSp - número de irmãos/esposa(o)
* Parch - número de pais/filhos
* Ticket - número do Ticket
* Fare - tarifa
* Cabin - cabine
* Embarked - porto de embarque (C = Cherbourg; Q = Queenstown; S = Southampton)

# Limpeza e Tratamento de dados

Foram disponibilizados 2 bases (treino e teste). As seguintes análises foram feitas:

* Foi criado a variável Título a partir do título contido no começo do nome dos passageiros

* PassengerId, Name e Ticket foram deletados por conter valores únicos

* Cabin foi deletada por possuir a maioria dos valores nulos

* Foi criada a variável Familiares a partir da soma das variáveis SibSp e Parch. Depois estas duas foram deletadas.

* Os valores nulos em Age foram preenchidos considerando a média das categorias em Título

* Foram criadas faixa de valores em Age e Fare

* Foram testados dois modelos de Machine Learning (DecisionTreeClassifier e RandomForestClassifier)

* Escolhido o melhor modelo e otimizá-lo

# Tecnologias utilizadas

* Jupyter Notebook
* Python
* Pandas
* Seaborn
* Scikit-learn
