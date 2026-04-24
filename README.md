## Detecção de Fraudes com Machine Learning
 Sobre o Projeto

Este projeto tem como objetivo identificar transações fraudulentas utilizando técnicas de Machine Learning. A proposta é construir um modelo capaz de detectar fraudes com alta precisão, minimizando falsos positivos e contribuindo para a redução de prejuízos financeiros.

## Dataset

Os dados utilizados são provenientes do Kaggle e representam transações financeiras anonimizadas.

Contém variáveis numéricas resultantes de transformação (PCA)
Classe altamente desbalanceada (fraudes são minoria)
Problema típico de classificação binária (fraude vs não fraude)

## Objetivo

Desenvolver um modelo preditivo capaz de:

Identificar fraudes com alta taxa de detecção (recall)
Minimizar falsos positivos
Simular um cenário realista de aplicação
## Etapas do Projeto
 1. Análise Exploratória (EDA)
Investigação da distribuição das variáveis
Análise do desbalanceamento das classes
Identificação de possíveis inconsistências
 2. Tratamento de Dados
Remoção de variáveis com data leakage (vazamento de informação)
Padronização e organização dos dados
Preparação para modelagem
 3. Modelagem

Foram testados diferentes algoritmos de Machine Learning:

- Random Forest

- XGBoost
  

Ajuste de hiperparâmetros com:


- RandomizedSearchCV


Tratamento de desbalanceamento:

- Uso de class_weight

## Avaliação dos Modelos

As métricas utilizadas foram:

- Recall (principal foco, devido ao contexto de fraude)

- Precision

- Matriz de confusão
  

# Melhor modelo: Random Forest

- Alta capacidade de detecção de fraudes (~98%)

- Baixo número de erros

- Ausência de falsos positivos (no cenário avaliado)

## Principais Insights
Pequenos vazamentos de dados (data leakage) podem inflar artificialmente a performance do modelo
O tratamento do desbalanceamento é essencial para problemas de fraude
Modelos mais simples, bem ajustados, podem superar alternativas mais complexas

## Tecnologias Utilizadas
- Python

- Pandas / NumPy

- Scikit-learn

- XGBoost

- Matplotlib / Seaborn


## Estrutura do Projeto
- notebooks/ → Análise e modelagem
- data/ → Base de dados

## Conclusão

O projeto demonstrou que é possível construir um modelo eficiente para detecção de fraudes utilizando técnicas de Machine Learning, desde que haja atenção especial à qualidade dos dados e ao tratamento de vieses.

Além do desempenho do modelo, o principal aprendizado foi a importância da análise crítica dos dados e das decisões tomadas ao longo do processo.

## Acesse o Projeto

👉 <(https://github.com/evellyrodrigues6-hash/Projeto_Semantix/blob/main/Projeto_Semantix.ipynb)>

## Contato
Projeto de Detecção de Fraudes
Sobre o projeto

Este projeto tem como objetivo detectar transações fraudulentas utilizando técnicas de machine learning. A proposta foi simular um cenário real, passando por todas as etapas de um projeto de dados: análise, tratamento, modelagem e avaliação.

Dados

O dataset utilizado é do Kaggle e representa transações financeiras anonimizadas.

Durante a análise inicial, foi possível observar:

forte desbalanceamento entre as classes
variáveis já transformadas (PCA)
necessidade de cuidado com possíveis vieses
Análise e pré-processamento

Na etapa exploratória, identifiquei que algumas variáveis estavam influenciando diretamente o resultado do modelo (data leakage). Para evitar um desempenho artificialmente alto, removi essas colunas:

device_risk_score
ip_risk_score
country_ng

Também foram realizadas:

conversão de variáveis categóricas
padronização dos dados
tratamento do desbalanceamento com class_weight
Modelagem

Foram testados dois modelos principais:

Random Forest
XGBoost

Para melhorar os resultados, utilizei o RandomizedSearchCV na busca de hiperparâmetros mais adequados, reduzindo o tempo de processamento.

Resultados
Random Forest (modelo final)
Acurácia: 100%
Recall (fraudes): 98%
Precision (fraudes): 100%
Apenas 2 fraudes não detectadas
Nenhum falso positivo
XGBoost
Acurácia: 100%
Recall: 96%
Precision: 98%

O Random Forest apresentou melhor desempenho na detecção de fraudes.

Visualizações

O projeto inclui gráficos comparando os modelos e suas métricas, facilitando a análise de desempenho e a escolha do modelo final.

Principais aprendizados
Vazamento de dados pode distorcer o desempenho do modelo
O tratamento do desbalanceamento é essencial em problemas de fraude
Modelos bem ajustados podem superar alternativas mais complexas
Tecnologias utilizadas
Python
Pandas
Scikit-learn
XGBoost
Matplotlib / Seaborn
Conclusão

O projeto demonstra a importância da qualidade dos dados e do pré-processamento na construção de modelos confiáveis. O foco foi desenvolver uma solução com bom desempenho e mais próxima de um cenário real.

Acesse o projeto

https://github.com/evellyrodrigues6-hash/Projeto_Semantix

Contato

Fique à vontade para entrar em contato para sugestões ou troca de ideias.😊
