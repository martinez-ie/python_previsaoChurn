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
