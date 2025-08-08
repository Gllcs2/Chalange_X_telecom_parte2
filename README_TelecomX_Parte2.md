# 📊 Predição de Rotatividade de Clientes (Churn)

## 🚀 Visão Geral
Este projeto implementa um pipeline de **Machine Learning** para prever clientes com alta probabilidade de cancelar um serviço (rotatividade).  
O objetivo é fornecer uma ferramenta de apoio para estratégias de retenção, baseada em dados históricos.

O processo envolve:
- Análise exploratória inicial.
- Pré-processamento de dados numéricos e categóricos.
- Balanceamento de classes com **SMOTE**.
- Treinamento de modelos **Random Forest** e **Gradient Boosting**.
- Avaliação detalhada dos resultados e análise de variáveis mais relevantes.

---

## 🔧 Tecnologias Utilizadas
- **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Imbalanced-learn)
- **Jupyter Notebook** ou **Google Colab**
- **Machine Learning** (modelos ensemble)
- **SMOTE** para balanceamento de classes

---

## 📂 Estrutura do Projeto
```bash
├── dados_df.csv                   # Dataset principal
├── TelecomX_Parte2.ipynb          # Notebook com análise completa
├── README.md                      # Documentação do projeto
```

---

## 🔄 Fluxo de Trabalho
1. **Carregamento e inspeção inicial**  
   Visualização das primeiras linhas, tipos de dados e estatísticas básicas.

2. **Análise exploratória**  
   - Identificação de valores ausentes.  
   - Distribuição da variável alvo (Rotatividade).

3. **Pré-processamento**  
   - Normalização de variáveis numéricas.
   - One-Hot Encoding para variáveis categóricas.
   - Balanceamento com SMOTE no conjunto de treino.

4. **Modelagem**  
   - Treinamento de Random Forest e Gradient Boosting.

5. **Avaliação**  
   - Relatórios de classificação.  
   - Matrizes de confusão.  
   - Curvas ROC comparativas.

6. **Importância das variáveis**  
   - Top 15 variáveis mais influentes para cada modelo.

7. **Conclusões**  
   - Interpretação dos resultados e próximos passos.

---

## 📈 Principais Resultados
| Modelo           | AUC Score |
|------------------|-----------|
| Random Forest    | ~0.83     |
| Gradient Boosting| ~0.84     |

- O **Gradient Boosting** teve leve vantagem em sensibilidade para prever clientes de risco.
- O **SMOTE** melhorou o equilíbrio das classes no treinamento.
- Algumas variáveis se destacaram como fortes preditoras, como `Charges.Total` e `Estágio`.

---

## 🚀 Próximos Passos
- Testar outros algoritmos como XGBoost ou LightGBM.
- Criar dashboard interativo para visualização em tempo real.
- Automatizar a atualização do modelo.

---

## 👨‍💻 Autor
**Gabriel Lucas Maia**
