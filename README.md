<p align="center">
  <img src="https://github.com/martinez-ie/python_previsaoChurn/blob/main/imagens/banner_churn.png" alt="Banner do Projeto" width="100%">
</p>

# 🎬 Previsão de Churn em Plataforma de Streaming

Este projeto tem como objetivo prever quais usuários de uma plataforma de streaming têm maior probabilidade de cancelar a assinatura (churn), utilizando algoritmos de **classificação supervisionada**. É um exemplo prático de como a ciência de dados pode apoiar estratégias de retenção de clientes.

---

## 📌 Índice

- [🎯 Objetivo](#-objetivo)
- [🧪 Etapas do Projeto](#-etapas-do-projeto)
- [🛠️ Tecnologias e Bibliotecas Utilizadas](#️-tecnologias-e-bibliotecas-utilizadas)
- [📈 Resultados](#-resultados)
- [💡 Aprendizados](#-aprendizados)
- [🔗 Acesse](#-acesse)

---

## 🎯 Objetivo

Identificar o perfil de usuários com maior risco de churn e treinar modelos de classificação para antever cancelamentos com base em dados históricos da plataforma.

---

## 🧪 Etapas do Projeto

1. **Análise Exploratória de Dados (EDA)**
   - Leitura do dataset
   - Verificação de valores nulos, tipos de dados e estatísticas descritivas
   - Visualizações com `seaborn` (baseadas no Python Graph Gallery)

2. **Limpeza e Pré-processamento**
   - Remoção/substituição de nulos
   - Codificação com `get_dummies` e `LabelEncoder`
   - Normalização com `MinMaxScaler`

3. **Modelagem**
   - Aplicação da **Regressão Logística** como baseline
   - Avaliação com `ConfusionMatrixDisplay` e `classification_report`

4. **Tuning**
   - Implementação de **RandomForestClassifier**
   - Estrutura clara com `fit`, `predict`, `assign`

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

- **Python** (Jupyter Notebook)
- **pandas**, **numpy**
- **seaborn**, **matplotlib**
- **scikit-learn**

---

## 📈 Resultados

A combinação entre as variáveis selecionadas e os modelos aplicados permitiu identificar padrões claros de comportamento dos usuários. O modelo Random Forest apresentou melhor desempenho em relação à regressão logística.

---

## 💡 Aprendizados

- Estruturação de um pipeline de machine learning supervisionado.
- Comparação entre modelos de classificação.
- Aplicação prática de estratégias de retenção orientadas a dados.

---

## 🔗 Acesse

📂 [Repositório no GitHub](https://github.com/martinez-ie/python_previsaoChurn)
