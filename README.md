# 📌 Projeto: Classificação de Inadimplentes com Machine Learning

Este projeto tem como objetivo entender os fatores que levam à **inadimplência de clientes** e desenvolver um **modelo preditivo** para auxiliar instituições financeiras na gestão de crédito. A abordagem inclui desde a análise exploratória até a otimização do modelo, utilizando técnicas avançadas de Machine Learning e Engenharia de Features.

## 🎯 Objetivos

- **Analisar fatores** que influenciam a inadimplência.
- **Identificar variáveis relevantes** para prever o comportamento financeiro dos clientes.
- **Criar e otimizar um modelo de classificação**, focando na redução de falsos negativos.
- **Gerar insights acionáveis** para aprimorar a gestão de risco financeiro.

## 📂 Estrutura do Projeto

```
├── 📂 data                                          # Backup do dataset
├── Projeto-ML-Classificacao-de-Inadimplentes.ipynb  # Notebook principal com todo o pipeline
├── README.md                                        # Este arquivo
```

## 🔧 Tecnologias Utilizadas

- **Linguagem**: Python
- **Bibliotecas**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `XGBoost`, `imbalanced-learn`
- **Ferramentas**: Google Colab, Google Cloud Storage, GitHub
- **Técnicas Aplicadas**: **SMOTE**, **Feature Engineering**, **PCA**, **GridSearchCV**

## 📊 Etapas do Projeto

1. **Aquisição de Dados**  
   - Importação de dataset de clientes.
   - Tratamento de valores ausentes e inconsistências.

2. **Análise Exploratória (EDA)**  
   - Identificação de padrões entre clientes adimplentes e inadimplentes.  
   - Visualização das principais variáveis categóricas e numéricas.  

3. **Engenharia de Features**  
   - **Criação de novas variáveis** como taxa de utilização de crédito, média de transações e intensidade de interações.  
   - **Transformações**: Label Encoding, One-Hot Encoding e normalização dos dados.  

4. **Modelagem e Treinamento**  
   - Teste de modelos iniciais: **Regressão Logística, Árvore de Decisão, Random Forest e XGBoost**.  
   - Aplicação de **SMOTE** para balanceamento das classes.  
   - **Otimização do XGBoost** com GridSearchCV.  

5. **Avaliação e Interpretação**  
   - **Métricas de performance**: Recall, AUC-ROC, F1-Score.  
   - **Análise de matriz de confusão** para entender erros do modelo.  
   - **Importância das features** para entender os principais fatores de inadimplência.  

## 📈 Principais Resultados

- O **XGBoost otimizado** apresentou os melhores resultados, equilibrando recall e precisão.
- A **quantidade de transações** e a **média do valor transacionado** foram variáveis cruciais para a previsão.
- Clientes com **maior tempo de inatividade** e **menor uso do crédito disponível** têm maior risco de inadimplência.

## 🚀 Próximos Passos

- Implementação de **LightGBM e CatBoost** para comparação de desempenho.  
- Refinamento do **threshold de decisão** para reduzir falsos negativos.  
- Exploração de **técnicas de Explainable AI (SHAP/LIME)** para interpretar melhor as previsões.  

## 🤝 Contribuições

Se quiser contribuir, sinta-se à vontade para abrir uma **issue** ou enviar um **pull request**. Qualquer sugestão para melhorias será bem-vinda!

## 📄 Licença

Este projeto está sob a licença **MIT**. Consulte o arquivo LICENSE para mais detalhes.
