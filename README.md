# Classificação usando modelo Logístico e variando o limiar de decisão

## Objetivo
Encontrar o threshold (limiar de decisão) que produz o melhor valor de F1-score para o modelo.

## Etapas
- Importar as bibliotecas;
- Carregar o dataset;
- Dividir os dados em treino e teste;
- Treinar o modelo de Regressão Logistica;
- Gerar previsões com threshold 0.5;
- Construir a matriz de confusão;
- Plotar a curva ROC e calcular AUC;
- Encontrar o melhor threshold
- - Criar uma lista de cortes entre 0 e 1;
- - Para cada corte, calcular as previsoes e a matriz de confusão;
- - Calcular as métricas: precisão, recall, f1-score;
- - Armazenar o F1-score para cada valor de corte;
- - Refazer a matriz de confusão para o melhor corte.
    