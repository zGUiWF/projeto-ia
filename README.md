# Projeto de IA: Predição de Evasão Acadêmica com XAI

Este projeto tem como objetivo aplicar técnicas de Machine Learning (ML) e Inteligência Artificial (IA) para prever a evasão de alunos com base em dados educacionais. Utilizamos um pipeline completo que vai desde a análise exploratória até a explicação dos modelos utilizando técnicas de XAI (eXplainable AI).

## 📊 Visão Geral

O modelo é treinado a partir de um conjunto de dados contendo informações de acesso, engajamento e dados pessoais dos alunos. O foco é identificar padrões de evasão e aplicar modelos de classificação para prever quais alunos têm maior risco de abandonar a plataforma de ensino.

## 🧪 Etapas do Projeto

1. **Importação de bibliotecas e dados**  
   Carregamento dos principais DataFrames utilizados para análise.

2. **Análise Exploratória e Pré-processamento**  
   - Visualização de dados base  
   - Conversão de timestamps  
   - Tratamento de valores faltantes por três abordagens (com destaque para o método final utilizado)  
   - Remoção de dados irrelevantes  
   - Feature Engineering e seleção de variáveis

3. **Definição de Lógica de Evasão**  
   - Alunos ausentes por 30 dias (fora do período de férias)
   - Alunos que iniciaram mas ficaram inativos por mais de 15 dias

4. **Modelagem Preditiva**  
   - Random Forest Classifier  
   - XGBoost Classifier  
   - Comparação entre os modelos em métricas como Acurácia, Precisão e Recall

5. **Interpretação com XAI**  
   Técnicas explicáveis foram utilizadas para justificar as decisões dos modelos, promovendo transparência.

## 🧠 Modelos Utilizados

- `RandomForestClassifier`
- `XGBoostClassifier`

Ambos foram avaliados e comparados quanto ao seu desempenho preditivo e interpretabilidade.

## 🧰 Tecnologias e Bibliotecas

- Python 3.10+
- Pandas
- NumPy
- scikit-learn
- XGBoost
- Matplotlib / Seaborn
