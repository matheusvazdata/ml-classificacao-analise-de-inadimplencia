# 📌 Projeto: Análise de Inadimplência e Comportamento Financeiro

Este projeto visa identificar padrões que levam à inadimplência de clientes e construir um modelo preditivo para auxiliar instituições financeiras na gestão de crédito e mitigação de riscos. A análise considera variáveis financeiras, comportamentais e socioeconômicas para melhorar a tomada de decisões estratégicas.

## 🎯 Objetivos

- Analisar fatores que influenciam a inadimplência.
- Identificar variáveis relevantes para prever o comportamento financeiro dos clientes.
- Construir e otimizar um modelo de Machine Learning para classificação de inadimplentes.
- Fornecer insights acionáveis para aprimorar a gestão de risco financeiro.

## 📂 Estrutura do Projeto

├── data/                 # Dados brutos e processados <br>
├── notebooks/            # Notebooks Jupyter com a análise exploratória e desenvolvimento do modelo <br>
├── README.md             # Documento atual

## 🔧 Tecnologias Utilizadas

- **Linguagem**: Python
- **Bibliotecas**: pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost, imbalanced-learn
- **Ferramentas**: Google Colab, Google Cloud Storage, GitHub
- **Técnicas Avançadas**: PCA, RandomizedSearchCV

## 📊 Etapas do Projeto

1. Aquisição de Dados: Coleta de informações financeiras dos clientes.
2. Tratamento de Dados: Limpeza e preparação dos dados para análise.
3. Análise Exploratória: Visualização de padrões e correlações.
4. (**Em construção**) Engenharia de Features: Seleção e transformação das variáveis.
5. Modelagem: Treinamento e validação de modelos de classificação.
6. Avaliação de Performance: Métricas como acurácia, recall e F1-score.
7. (**Em construção**) Interpretação e Conclusão: Discussão dos resultados e sugestões para aplicação.

## 📈 Principais Resultados

- O modelo **XGBoost** apresentou os melhores resultados, sendo otimizado para minimizar falsos negativos.
- Variáveis como **quantidade de transações**, **valor médio de transações** e **tempo de relacionamento com a instituição** foram cruciais para a classificação.

## 🚀 Próximos Passos

- Implementação de **LightGBM e CatBoost** para comparação de desempenho.
- Ajuste fino no threshold para maximizar recall sem comprometer a precisão.
- Técnicas como **SMOTE** e ajuste de **threshold** ajudaram a melhorar a detecção de inadimplentes.

## 🤝 Contribuições

Contribuições são bem-vindas! Caso tenha sugestões de melhorias ou queira colaborar, abra uma **issue** ou envie um **pull request**.

## 📄 Licença

Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.
