# FIAP Tech Challenge - Fase 3
## ✈️ Análise e Previsão de Atrasos de Voos com Machine Learning

Projeto da fase 3 da pós em Machine Learning Engineering focado na análise exploratória e modelagem preditiva de atrasos de voos nos Estados Unidos, utilizando técnicas de Machine Learning supervisionado.

## 🎯 Objetivo do Projeto

Desenvolver um pipeline completo de análise de dados capaz de:

- Explorar e entender os dados de voos (EDA)
- Identificar padrões e fatores relacionados a atrasos
- Tratar valores ausentes de forma adequada
- Construir modelos de Machine Learning para previsão de atrasos
- Avaliar e comparar diferentes algoritmos

## 📊 Base de Dados

O projeto utiliza três datasets principais:

- **flights.csv** → informações dos voos (atrasos, horários, distâncias)
- **airlines.csv** → identificação das companhias aéreas
- **airports.csv** → informações dos aeroportos (cidade, estado, etc.)

Essas bases foram integradas para enriquecer a análise.

## 🧠 Etapas do Projeto

### 🔹 1. Integração dos Dados
- Merge das bases `flights`, `airlines` e `airports`
- Criação de dataset consolidado

### 🔹 2. Análise Exploratória (EDA)
- Estatísticas descritivas
- Visualizações de dados
- Identificação de padrões de atraso por:
  - companhia aérea
  - aeroporto
  - dia da semana
  - horário

### 🔹 3. Tratamento de Dados
- Remoção de voos cancelados
- Tratamento de valores ausentes com base no contexto
- Criação das variáveis alvo:
  - `IS_DELAYED` (classificação)
  - `ARRIVAL_DELAY` (regressão)

### 🔹 4. Modelagem Supervisionada

#### 📌 Classificação
Objetivo: prever se um voo irá atrasar ou não.

Modelos utilizados:
- Logistic Regression
- Decision Tree

#### 📌 Regressão
Objetivo: prever o tempo de atraso do voo (em minutos).

Modelos utilizados:
- Linear Regression (baseline)
- (opcional: Decision Tree Regressor / Random Forest Regressor)

## 📈 Avaliação dos Modelos

### Classificação:
- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusão

### Regressão:
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score
