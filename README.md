# FIAP Tech Challenge - Fase 3
## ✈️ Análise e Previsão de Atrasos de Voos com Machine Learning

Projeto da fase 3 da pós em Machine Learning Engineering focado na análise exploratória e modelagem preditiva de atrasos de voos nos Estados Unidos, utilizando técnicas de Machine Learning supervisionado e não supervisionado.

## 🎯 Objetivo do Projeto

Desenvolver um pipeline completo de análise de dados capaz de:

- Explorar e entender os dados de voos (EDA)
- Identificar padrões e fatores relacionados a atrasos
- Tratar valores ausentes de forma adequada
- Construir modelos de Machine Learning para previsão de atrasos
- Aplicar técnicas de aprendizado não supervisionado para identificar padrões ocultos
- Avaliar e interpretar os resultados

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

---

### 🔹 3. Tratamento de Dados
- Remoção de voos cancelados
- Tratamento de valores ausentes com base no contexto
- Criação da variável alvo:
  - `IS_DELAYED` (classificação)

### 🔹 4. Modelagem Supervisionada

#### 📌 Classificação
Objetivo: prever se um voo irá atrasar ou não.

Modelos utilizados:
- Logistic Regression
- Decision Tree

### 🔹 5. Modelagem Não Supervisionada

#### 📌 Clusterização (K-Means)

Objetivo: identificar padrões e agrupar voos com características semelhantes.

Etapas realizadas:
- Seleção de variáveis numéricas relevantes
- Padronização dos dados
- Definição do número de clusters (Elbow Method)
- Aplicação do algoritmo K-Means
- Redução de dimensionalidade com PCA para visualização

## 📈 Avaliação dos Modelos

### Classificação:
- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusão

### Clusterização:
- Análise visual dos clusters (PCA)
- Interpretação dos grupos formados

## 📌 Principais Insights

- Atrasos variam significativamente entre companhias aéreas
- Alguns aeroportos apresentam maior incidência de atrasos
- Horários ao longo do dia influenciam a probabilidade de atraso
- A clusterização revelou diferentes perfis de voos com comportamentos distintos

## 📌 Conclusão

O projeto demonstrou que os atrasos de voos não ocorrem de forma aleatória, estando associados a fatores como companhia aérea, horário e características operacionais.

A modelagem supervisionada mostrou que é possível prever a ocorrência de atrasos com base em dados históricos, enquanto a clusterização permitiu identificar diferentes perfis de voos, evidenciando padrões ocultos nos dados.

Essas abordagens complementares contribuem para uma compreensão mais completa do problema, podendo apoiar análises e decisões no contexto operacional.
