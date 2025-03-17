# 📌 Projeto: Classificação de Inadimplentes com Machine Learning  

Este projeto tem como objetivo entender os fatores que levam à **inadimplência de clientes** e desenvolver um **modelo preditivo** para auxiliar instituições financeiras na gestão de crédito. A abordagem inclui desde a análise exploratória até a otimização do modelo, utilizando técnicas avançadas de Machine Learning e Engenharia de Features.  

📊 **Apresentação do projeto:** [Clique aqui para visualizar no Figma](https://www.figma.com/proto/l2KkgCy2JepSTk3RD4jnoa/Projeto-de-Classifica%C3%A7%C3%A3o?node-id=115-2&p=f&t=ApAwrhxeZpVb4j37-1&scaling=contain&content-scaling=fixed&page-id=0%3A1)  

## 🎯 Objetivos  

- **Analisar fatores** que influenciam a inadimplência.  
- **Identificar variáveis relevantes** para prever o comportamento financeiro dos clientes.  
- **Criar e otimizar um modelo de classificação**, focando na redução de falsos negativos.  
- **Gerar insights acionáveis** para aprimorar a gestão de risco financeiro.  

## 📂 Estrutura do Projeto  

```
├── 📂 data
├── Projeto-ML-Classificacao-de-Inadimplentes.ipynb  # Notebook principal com todo o pipeline
├── README.md                                        # Este arquivo
```

## 🔧 Tecnologias Utilizadas  

- **Linguagem**: Python  
- **Bibliotecas**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `XGBoost`, `imbalanced-learn`  
- **Ferramentas**: Google Colab, Google Cloud Storage, GitHub  
- **Técnicas Aplicadas**: **SMOTE**, **Feature Engineering**, **PCA**, **GridSearchCV**  

## 📊 Etapas do Projeto  

1️⃣ **Aquisição de Dados**  
   - Importação do dataset de clientes.  
   - Tratamento de valores ausentes e inconsistências.  

2️⃣ **Análise Exploratória (EDA)**  
   - Identificação de padrões entre clientes **adimplentes e inadimplentes**.  
   - Visualização das principais variáveis categóricas e numéricas.  

3️⃣ **Engenharia de Features**  
   - **Criação de novas variáveis** como taxa de utilização de crédito, média de transações e intensidade de interações.  
   - **Transformações**: Label Encoding, One-Hot Encoding e normalização dos dados.  

4️⃣ **Balanceamento das Classes com SMOTE**  
   - O dataset apresentou um desbalanceamento significativo entre **inadimplentes (1)** e **adimplentes (0)**.  
   - Aplicação do **SMOTE (Synthetic Minority Over-sampling Technique)** para gerar novas amostras sintéticas e equilibrar a proporção das classes.  
   - A estratégia ajudou a melhorar a capacidade do modelo de identificar clientes inadimplentes.  

5️⃣ **Modelagem e Treinamento**  
   - Teste de modelos iniciais: **Regressão Logística, Árvore de Decisão, Random Forest e XGBoost**.  
   - **Otimização do XGBoost** com GridSearchCV para encontrar os melhores hiperparâmetros.  

6️⃣ **Avaliação e Interpretação**  
   - **Métricas de performance**: Recall, AUC-ROC, F1-Score.  
   - **Análise da matriz de confusão** para entender erros do modelo.  
   - **Importância das features** para entender os principais fatores de inadimplência.  

## 📈 Principais Resultados  

- O **XGBoost otimizado** apresentou os melhores resultados, equilibrando recall e precisão.  
- A **quantidade de transações** e a **média do valor transacionado** foram variáveis cruciais para a previsão.  
- Clientes com **maior tempo de inatividade** e **menor uso do crédito disponível** têm maior risco de inadimplência.  
- **SMOTE ajudou a reduzir o viés do modelo contra a classe minoritária (inadimplentes)**, melhorando a taxa de detecção de clientes de risco.  

## 🚀 Próximos Passos  

- Implementação de **LightGBM e CatBoost** para comparação de desempenho.  
- Refinamento do **threshold de decisão** para reduzir falsos negativos.  
- Exploração de **técnicas de Explainable AI (SHAP/LIME)** para interpretar melhor as previsões.  

## 🤝 Contribuições  

Se quiser contribuir, sinta-se à vontade para abrir uma **issue** ou enviar um **pull request**. Qualquer sugestão para melhorias será bem-vinda!  

## 📄 Licença  

Este projeto está sob a licença **MIT**. Consulte o arquivo LICENSE para mais detalhes.
