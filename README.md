# 🎯 Streaming Churn Prediction

Este projeto tem como objetivo prever quais usuários de uma plataforma de streaming têm maior chance de cancelar sua assinatura (churn), utilizando algoritmos de classificação supervisionada.

---

## 📌 Objetivo

Identificar o perfil dos usuários com maior probabilidade de sair da plataforma, permitindo que o negócio implemente ações preventivas e estratégias de retenção mais assertivas.

---

## 🧪 Etapas do Projeto

### 1. Análise Exploratória (EDA)
- Leitura do dataset.
- Estatísticas descritivas (`describe`, `info`, `isna().sum()`).
- Gráficos de distribuição com `seaborn`, baseados no [Python Graph Gallery](https://python-graph-gallery.com/).

### 2. Limpeza e Pré-processamento
- Substituição e remoção de valores nulos.
- Codificação de variáveis categóricas com `get_dummies` e `LabelEncoder`.
- Normalização com `MinMaxScaler`.

### 3. Modelagem Base
- Aplicação de **Regressão Logística** como modelo baseline.
- Avaliação com matriz de confusão e `classification_report`.

### 4. Tuning Supervisionado
- Aplicação de `RandomForestClassifier` com separação clara de cada função exigida (`fit`, `predict`, `assign`, `ConfusionMatrixDisplay`).

### 5. Modelagem Otimizada com GridSearchCV
- Busca pelos melhores hiperparâmetros com `GridSearchCV`.
- Avaliação e comparação final.

### 6. Análise de Perfil
- Extração das variáveis mais influentes para o churn com `feature_importances_`.
- Visualização com `barplot` (palette `viridis`).
- Conclusão estratégica com base nas variáveis mais relevantes.

---

## 🔍 Resultados

**Top 5 variáveis mais relevantes para o churn:**
1. `Num_active_profiles`
2. `Gender_Male`
3. `Devices_connected`
4. `Subscription_type_Premium`
5. `Subscription_type_Standard`

**Perfil com maior risco de churn:**
- Usuários com poucos perfis ativos,
- Do sexo masculino,
- Poucos dispositivos conectados,
- Mesmo em planos pagos como Premium ou Standard.

---

## 💼 Tecnologias Utilizadas

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-Learn

English version

🎯 Streaming Churn Prediction
This project aims to predict which users of a streaming platform are most likely to cancel their subscription (churn), using supervised classification algorithms.

📌 Objective
Identify the profile of users most likely to leave the platform, enabling the business to implement preventive actions and more effective retention strategies.

🧪 Project Steps

Exploratory Data Analysis (EDA)

Dataset loading

Descriptive statistics (describe, info, isna().sum())

Distribution plots using Seaborn, inspired by the Python Graph Gallery

Cleaning and Preprocessing

Handling and removing missing values

Encoding categorical variables with get_dummies and LabelEncoder

Normalization with MinMaxScaler

Baseline Modeling

Logistic Regression applied as the baseline model

Evaluation using confusion matrix and classification_report

Supervised Tuning

RandomForestClassifier applied with clear separation of tasks (fit, predict, assign, ConfusionMatrixDisplay)

Optimized Modeling with GridSearchCV

Hyperparameter tuning using GridSearchCV

Final evaluation and comparison

Profile Analysis

Extraction of the most influential variables for churn using feature_importances_

Visualization with barplot (viridis palette)

Strategic conclusion based on the most relevant features

🔍 Results
Top 5 most relevant variables for churn:

Num_active_profiles

Gender_Male

Devices_connected

Subscription_type_Premium

Subscription_type_Standard

Highest risk churn profile:

Users with few active profiles

Male users

Few connected devices

Even when subscribed to paid plans like Premium or Standard

💼 Technologies Used

Python

Pandas, NumPy

Seaborn, Matplotlib

Scikit-Learn
