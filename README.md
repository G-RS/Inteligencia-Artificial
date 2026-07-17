## 🧠 Inteligência Artificial

Este repositório contém uma coleção de sete projetos desenvolvidos com foco na aplicação de algoritmos de **Machine Learning** e **Processamento de Linguagem Natural (NLP)**. Os projetos abrangem desde a análise exploratória e preparação de dados, até a construção, validação e otimização de modelos preditivos para **Classificação**, **Regressão** e **Clusterização**. Através destes projetos, são exploradas técnicas avançadas de pré-processamento, balanceamento de dados, validação cruzada, otimização de hiperparâmetros e implementação de aplicações web interativas, visando extrair informações valiosas e automatizar processos de decisão.

<br>

## 💻 Tecnologias

As principais ferramentas e bibliotecas utilizadas nos projetos são:
* Linguagem: `Python`
* Ambiente: `Google Colab`, `Visual Studio Code`
* Bibliotecas: `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`, `Plotly`, `Scikit-Learn`, `Imbalanced-Learn`, `Scikit-Optimize`, `NLTK`, `WordCloud`, `Streamlit`, `Joblib`

<br>

## 📝 Conteúdo dos Notebooks

### **Classificação: Aprendendo a classificar dados com Machine Learning**
Focado nos conceitos iniciais de **Machine Learning**, aborda a análise exploratória e transformações de variáveis categóricas usando o `OneHotEncoder` e `LabelEncoder`. O projeto utiliza dados de uma campanha de marketing para aderência de investimentos e foca no treinamento de modelos para prever categorias, começando com o *baseline* `DummyClassifier`, evoluindo para a **Árvore de Decisão** (`DecisionTreeClassifier`) e comparando o desempenho com o método dos vizinhos mais próximos (`KNeighborsClassifier`). O modelo é persistido em disco utilizando a biblioteca `pickle`.

### **Classificação: Validação de modelos e métricas de avaliação**
Voltado à avaliação crítica dos resultados de **Machine Learning**, explora a base de dados de uma empresa de empréstimo de automóveis com clientes inadimplentes e adimplentes e também dados de pacientes com e sem diabetes. Aborda a validação de modelos com divisão em treino, validação e teste, assim como o método robusto de validação cruzada (`KFold` e `StratifiedKFold`). Explora diferentes métricas de performance através do `classification_report`, analisando a acurácia, precisão, recall e f1-score usando a matriz de confusão. Adicionalmente, trata o problema de dados desbalanceados com técnicas de *oversampling* (`SMOTE`) e *undersampling* (`NearMiss`), incorporando o `Pipeline` do `imblearn`.

### **Classificação: Resolvendo problemas multiclasse**
Neste projeto, o foco está na classificação de múltiplas categorias simultaneamente, com base em dados de estudantes, incluindo dados demográficos, socioeconômicos e macroeconômicos capturados no momento da matrícula e dados de classificação de vinhos. A análise exploratória inclui gráficos de distribuição e frequência. Em seguida, os dados são preparados e divididos para o treinamento do modelo de **Random Forest** (`RandomForestClassifier`). São avaliadas as saídas da classificação multiclasse, os impactos do balanceamento de dados, a definição da profundidade máxima das árvores e o cálculo de intervalos de confiança através da validação cruzada.

### **Classificação: Otimizando modelos de machine learning**
Destinado a melhorar o desempenho e extrair o máximo de algoritmos preditivos como **Árvore de Decisão**, **Regressão Logística** e **KNN**. Utiliza os dados de perfil de crédito para introduzir métodos avançados de busca pelo espaço de hiperparâmetros. Aplica a busca exaustiva via `GridSearchCV`, a busca randômica via `RandomizedSearchCV` com testes estatísticos, e finaliza com a otimização bayesiana da biblioteca `skopt` através do `BayesSearchCV`, sempre acompanhados de validação cruzada aninhada para avaliar a eficácia.

### **Regressão: Construindo Árvores de Regressão**
Focado no universo de problemas de **Regressão**, trabalha com uma base de dados de logística e entregas para prever valores contínuos referentes ao custo de entrega. Apresenta o detalhado tratamento de variáveis temporais (extração de dias, meses, anos e cálculo do tempo de entrega a partir de datas de agendamento e conclusão) e a codificação de variáveis categóricas (`get_dummies`), treinando modelos preditivos baseados em árvores: o `DecisionTreeRegressor` e a evolução para múltiplos estimadores com o `RandomForestRegressor`. O foco se concentra na avaliação do modelo usando métricas de erro, prevenção de *overfitting*, ajuste de hiperparâmetros com `GridSearchCV` e uso da validação cruzada.

### **Clusterização: Lidando com dados sem rótulo**
Explora a vertente da aprendizagem não supervisionada aplicados a dados de marketing. Aborda o agrupamento dos consumidores por seus temas de interesse através do algoritmo **K-Means**. Utiliza métricas como a inércia e o índice de silhueta (`silhouette_score`) apoiados pelo método do cotovelo para determinar a quantidade ótima de *clusters*. O projeto inclui a transformação e o reescalonamento dos dados (`MinMaxScaler`). Ao final, o modelo validado é implementado em uma aplicação web desenvolvida com `Streamlit`, permitindo inferências para novos conjuntos de dados.

### **NLP: Aplicando processamento de linguagem natural para análise de sentimentos**
Apresenta o domínio de **Processamento de Linguagem Natural** utilizando dados de avaliações textuais para identificar sentimentos (positivos ou negativos). Demonstra o pré-processamento de textos aplicando técnicas como *Bag of Words*, remoção de *stopwords* com a biblioteca `NLTK`, remoção de pontuação, *stemming* e tokenização. Visualiza os termos mais recorrentes usando `WordCloud`. O modelo utilizado para a classificação baseia-se em regressão logística treinado sobre representações textuais baseadas na relevância e contexto criadas com *TF-IDF* e *N-grams*.
