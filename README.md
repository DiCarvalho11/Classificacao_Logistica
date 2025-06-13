# Classificação usando modelo Logístico e variando o limiar de decisão

## Objetivo
Encontrar o threshold (limiar de decisão) que produz o melhor valor de F1-score para o modelo.

### Por que usar F1-score?
Porque ele é uma média harmônica entre precisão e recall, ideal para dados desbalanceados.

## Etapas

### 1. Preparação
- Importar as bibliotecas necessárias;
- Carregar o dataset;

### 2. Pré-processamento dos dados
- Dividir os dados em conjuntos de treino e teste;

### 3. Treinamento do modelo
- Treinar o modelo de Regressão Logística com os dados de treino;

### 4. Avaliação inicial com threshold padrão (0.5)
- Gerar previsões com threshold igual a 0.5;
- Construir a matriz de confusão;
- Calcular as métricas: acurácia, precisão, recall e F1-score;
- Traçar a curva ROC e calcular a AUC (Área sob a Curva);

### 5. Otimização do threshold
- Criar uma lista de possíveis thresholds entre 0 e 1 (ex.: de 0.0 a 1.0 com passo 0.01);
- Para cada threshold:
  - Aplicar o corte nas probabilidades preditas;
  - Calcular a matriz de confusão;
  - Calcular precisão, recall e F1-score;
- Armazenar o F1-score correspondente a cada threshold;

### 6. Seleção do melhor corte
- Identificar o threshold que fornece o maior F1-score;
- Refazer a matriz de confusão utilizando esse melhor threshold;
- Apresentar as métricas finais com o threshold ótimo.

