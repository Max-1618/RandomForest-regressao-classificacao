# RandomForest-regressao-classificacao
Utilizando o algoritmo Random Forest para construir modelos de Regressão Linear Múltipla e Classificação

MODELO DE REGRESSÃO LINEAR

O objetivo é prever a temperatura máxima do dia (variável "actual").
O conjunto de dados (dataset) contém 348 observações e 9 variáveis (atributos).

Etapas de desenvolvimento do modelo:

1-Análise exploratória / Pré-processamento (importante! Foi utilizada a técnica "one-hot encoding" para transformar as variáveis
categóricas. Sendo assim, foram criadas as chamadas variáveis "dummies");
2-Criação do modelo de regressão RandomForestRegressor (instância com 100 árvores);
3-O modelo obteve um MAPE igual a 6.42% e acurácia de 93.57%;
4-Foram verificadas as variáveis mais relevantes (features importances);
5-Nova versão do modelo com apenas as duas variáveis mais importantes;
6-Resultado: MAPE igual a 6.59% e acurácia de 93.40% (ligeiramente inferior a primeira versão).

MODELO DE CLASSIFICAÇÃO

O objetivo é prever uma concessão de crédito (análise do risco de concessão). Variável alvo "default" (binária).
O conjunto de dados (dataset) contém 1000 observações com 17 variáveis (atributos). As classes não estão balanceadas.

Etapas de desenvolvimento do modelo:

1-Análise e Pré-processamento (One-hot encoding - variáveis dummies);
2-Criação de um modelo de árvore de decisão - DecisionTreeClassifier;
3-O modelo obteve 63% de acurácia, mas uma taxa de precisão de apenas 41% para a classe 1;
4-Verificação da relevância das variáveis (features importances);
5-Criação do modelo usando o algoritmo RandomForestClassifier (instância com 100 árvores);
6-O modelo obteve 75% de acurácia, com taxas de precisão de 79% e 62% para as classes 0 e 1 respectivamente;
7-Gravação do modelo (objeto).
8-Exemplo de como carregar o modelo (objeto).

IMPORTANTE! Alguns hiperparâmetros do algoritmo RandomForestClassifier foram alterados.




