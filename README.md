# Projeto de Detecção de Fraude

## Sobre

Esse projeto tem como objetivo identificar transações fraudulentas usando machine learning. Usei um dataset sintético do Kaggle e passei por todo o fluxo: exploração dos dados, tratamento, modelagem e avaliação.

---

## Dados e análise

* Dataset de fraude (Kaggle)
* Análise exploratória para entender distribuição e padrões
* Verificação de desbalanceamento entre as classes
* Ajuste de tipos de dados e padronização de categorias

---

## Pré-processamento

Durante a análise, percebi que algumas variáveis estavam influenciando demais o modelo. Para evitar viés e deixar o resultado mais realista, removi:

* device_risk_score
* ip_risk_score
* country_ng

Também transformei variáveis categóricas em numéricas e tratei o desbalanceamento usando `class_weight='balanced'`.

---

## Modelos

Testei dois modelos principais:

* Random Forest
* XGBoost

Para melhorar o desempenho, utilizei o **RandomizedSearchCV** para buscar bons hiperparâmetros sem precisar testar todas as combinações.

---

## Visualização dos Resultados

### Comparação dos Modelos

![Comparação dos Modelos](images/random_forest_vs_xgboost.png)

### Desempenho do XGBoost

![XGBoost](images/xgboost_resultados.png)

### Desempenho do Random Forest

![Random Forest](images/random_forest_resultados.png)

### Comparativo Final

![Comparativo Final](images/comparativo_final.png)

### Modelo Final

![Modelo Final](images/modelo_final.png)

---

## Resultados

### Random Forest (modelo escolhido)

* Acurácia: 100%
* Classe 0: 100% em todas as métricas
* Classe 1 (fraude):

  * Precisão: 100%
  * Recall: 98%
  * F1-score: 99%
* Apenas 2 fraudes não detectadas
* Nenhum falso positivo

### XGBoost

* Acurácia: 100%
* Classe 0: 100% em todas as métricas
* Classe 1 (fraude):

  * Precisão: 98%
  * Recall: 96%
  * F1-score: 97%

---

## Conclusões

Os dois modelos tiveram um desempenho muito bom, mas o Random Forest se saiu melhor na detecção de fraudes.

Um ponto importante foi perceber que resultados perfeitos podem indicar problema nos dados. Ao remover variáveis que “entregavam” a resposta, o modelo ficou mais confiável.

No geral, o projeto mostrou como o pré-processamento e a análise dos dados fazem muita diferença no resultado final.

---

## Tecnologias

* Python
* Pandas
* Scikit-learn
* XGBoost
* Random Forest

---

## Como usar

1. Clone o repositório
2. Instale as dependências
3. Execute o notebook principal

---

## Contato

Se quiser trocar ideia ou sugerir melhorias, fica à vontade para entrar em contato :)
