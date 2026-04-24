## Detecção de Fraudes com Machine Learning
 Sobre o Projeto

Este projeto tem como objetivo identificar transações fraudulentas utilizando técnicas de Machine Learning. A proposta é construir um modelo capaz de detectar fraudes com alta precisão, minimizando falsos positivos e contribuindo para a redução de prejuízos financeiros.

## Dataset

Os dados utilizados são provenientes do Kaggle e representam transações financeiras anonimizadas.

Contém variáveis numéricas resultantes de transformação (PCA)
Classe altamente desbalanceada (fraudes são minoria)
Problema típico de classificação binária (fraude vs não fraude)
 Objetivo

Desenvolver um modelo preditivo capaz de:

Identificar fraudes com alta taxa de detecção (recall)
Minimizar falsos positivos
Simular um cenário realista de aplicação
 Etapas do Projeto
 1. Análise Exploratória (EDA)
Investigação da distribuição das variáveis
Análise do desbalanceamento das classes
Identificação de possíveis inconsistências
 2. Tratamento de Dados
Remoção de variáveis com data leakage (vazamento de informação)
Padronização e organização dos dados
Preparação para modelagem
 3. Modelagem

## Foram testados diferentes algoritmos de Machine Learning:

Random Forest
XGBoost

## Ajuste de hiperparâmetros com:

RandomizedSearchCV

 # Tratamento de desbalanceamento:

Uso de class_weight
 Avaliação dos Modelos

## As métricas utilizadas foram:

Recall (principal foco, devido ao contexto de fraude)
Precision
Matriz de confusão

## Melhor modelo: Random Forest

Alta capacidade de detecção de fraudes (~98%)
Baixo número de erros
Ausência de falsos positivos (no cenário avaliado)
 Principais Insights
Pequenos vazamentos de dados (data leakage) podem inflar artificialmente a performance do modelo
O tratamento do desbalanceamento é essencial para problemas de fraude
Modelos mais simples, bem ajustados, podem superar alternativas mais complexas
## Tecnologias Utilizadas
Python
Pandas / NumPy
Scikit-learn
XGBoost
Matplotlib / Seaborn
 Estrutura do Projeto
notebooks/ → Análise e modelagem
data/ → Base de dados

## Conclusão

O projeto demonstrou que é possível construir um modelo eficiente para detecção de fraudes utilizando técnicas de Machine Learning, desde que haja atenção especial à qualidade dos dados e ao tratamento de vieses.

Além do desempenho do modelo, o principal aprendizado foi a importância da análise crítica dos dados e das decisões tomadas ao longo do processo.

## Acesse o Projeto

👉 <(https://github.com/evellyrodrigues6-hash/Projeto_Semantix/blob/main/Projeto_Semantix.ipynb)>

## Contato

Fique à vontade para contribuir ou trocar ideias sobre o projeto! 😊
