<img width="974" height="134" alt="image" src="https://github.com/user-attachments/assets/0a53a0bf-93ba-4ff5-a853-cf0914d6eb95" />

# Criatura lendária - Cubo gelatinoso 2026
<h1 align="center"> Previsão de diabetes com o modelo K-NN </h1>

**Aluna:** Ana Luiza de Lima Silva.

**Turma:** 2026

**Docente responsável:** Prof. Dr. Daniel Roberto Cassar

**Disciplina:** Aprendizado de máquina - 2° semestre de 2026.

**Instituição:** Ilum escola de ciência.

## Índice
<!--ts-->
* [Objetivo da atividade](##Objetivo-da-atividade)
* [Conjunto de dados](##Conjunto-de-dados)
* [Metodologias e análises empregadas](##Metodologias-e-análises-empregadas)
* [Instruções para uso](##Instruções-para-uso)
* [Bibliotecas utilizadas](##Bibliotecas-utilizadas)
* [Conclusões e resultados](##Conclusões-e-resultados)
* [Agradecimentos](##Agradecimentos)
* [Referências](##Referências)
* [Docente responsável](##Docentes-responsáveis)
* [Autoria](##Desenvolvedora)
<!--te-->

## Objetivo da atividade
<p align="justify"> Permitir um primeiro contato dos estudantes com modelos de Aprendizado de Máquina, em especial o K-NN, de modo a visualizar o desempenho e comportamento deste. Para isso serão avaliados como diferentes parâmetros aplicados a esse modelo influenciam e afetam seus resultados e previsões.

## Conjunto de dados
<p align="justify"> CDC Diabetes Health Indicators, disponibilizado pelo UCI Machine Learning Repository. Este Dataset é disponibilizado para implementação em Python diretamente pela biblioteca ucimlrepo, não sendo necessário instalar arquivos adicionais, mas sim apenas executar as células do notebook na ordem em que aparecem.

## Metodologias e análises empregadas
- Análise exploratória do conjunto de dados;
- Separação de uma amostra do conjunto de dados para ser utilizada durante o notebook, mantendo o desbalanceamento existente entre as classes;
- Implementação da estratégia de Holdout e separação em dados de treino e teste;
- Implementação do modelo K-NN;
- Verificação dos atributos com maior importância para o modelo;
- Variação dos hiperparâmetros e reconhecimento daquele que fornece as melhores previsões;
- Testes de normalização e codificação dos dados;
- Comparação a um modelo de Baseline;
- Verificação dos resultados a partir de diferentes métricas de desempenho.

## Instruções para uso
<p align="justify"> O único arquivo necessário para a execução do notebook é o notebook intitulado "Cubo Gelatinoso".


## Bibliotecas utilizadas
Os códigos utilizados para a realização da atividade foram desenvolvidos na linguagem de programação Python (3.13.7), contando com as seguintes bibliotecas e seus usos:

- Pandas (2.3.3): utilizada para a visualização e manipulação dos dados em DataFrames; 

- Seaborn (0.13.2): utilizada para a produção dos gráficos presentes no notebook;

- Matplotlib.pyplot (3.10.6): utilizada para melhorar a visualização de alguns dos gráficos;

- ucimlrepo: utilizada para importação do Dataset;

- O objeto "permutation_importance" da biblioteca Sklearn.inspection (1.7.2): utilizado para avaliar a importância de cada um dos atributos utilizados para o modelo;

- O objeto "train_test_split" da biblioteca Sklearn.model_selection (1.7.2): utilizado para realizar a divisão dos dados de treino e teste antes de efetivamente instanciar e treinar o modelo;

- O objeto "KNeighborsClassifier" da biblioteca Sklearn.neighbors (1.7.2): utilizado para implementar o algoritmo KNN;

- O objeto "DummyClassifier" da biblioteca Sklearn.dummy (1.7.2): utilizado para treinar o modelo de Baseline;

- O objeto "product" da bilioteca itertools: utilizado para realizar a variação dos conjuntos de hiperparâmetros apra avaliar o modelo KNN;

- Os objetos "accuracy_score", "confusion_matrix", "roc_auc_score", "precision_score", "recall_score", "f1_score", "roc_curve" da biblioteca Sklean.metrics: utilizados para comparar os resultados de diferentes métricas de desempenho. Cada um deles será explicado em detalhes na seção "Quais os resultados de diferentes métricas de desempenho?;

- Os objetos "StandardScaler", "MaxAbsScaler", "MinMaxScaler", "OneHotEncoder" da biblioteca Sklearn.preprocessing: utilizados na normalização e codificação dos dados. Serão explicados nas seções "Normalizando os dados e avaliando o algoritmo KNN", "Teste de hipótese - codificar os atributos alteraria os resultados?" e "Qual seria o resultado ao codificar e normalizar os dados?".


## Conclusões e resultados
- As avaliações foram conduzidas a partir de um Dataset desbalanceado, de modo que mesmo o modelo de Baseline apresenta uma acurácia elevada, de aproximadamente 86%. No entanto, avaliando outras métricas, como F1-score, esse modelo se mostrou insuficiente ao realizar as previsões;

- Os melhores resultados para o modelo KNN foram obtidas considerando 13 vizinhos, peso uniforme e distância Euclidiana;

- A única estratégia de pré-processamento que melhorou o desempenho do modelo foi a normalização usando o normalizador padrão StandardScaler.

## Agradecimentos
Agradeço ao professor docente responsável por ministrar a disciplina de Aprendizado de Máquina no segundo semestre letivo do ano de 2026 e por todo o suporte oferecido durante o desenvolvimento desta atividade.

## Referências 

[1] IBM. Aprendizado de máquina. Disponível em: <https://www.ibm.com/br-pt/think/topics/machine-learning>. Acesso em: 12 set. 2026.

[2] CASSAR, Daniel R. ATP-203 2.1 - Aprendizado de máquina, k-NN e métricas. 2026. Jupyter Notebook. Material didático não publicado.

[3] CASSAR, Daniel R. ATP-203 2.2 - Divisão de dados em treino e teste. 2026. Jupyter Notebook. Material didático não publicado.

[4] CHUGH, Vidhi. Pontuação F1 em machine learning: Uma métrica equilibrada para precisão e recuperação. Disponível em: <https://www.datacamp.com/pt/tutorial/f1-score>. Acesso em: 12 set. 2026.

[5] UCI Machine Learning Repository. Disponível em: <https://archive.ics.uci.edu/dataset/891/cdc%2Bdiabetes%2Bhealth%2Bindicators>. Acesso em: 24 ago. 2026.

[6] 1.6. Nearest Neighbors. Disponível em: <https://scikit-learn.org/stable/modules/neighbors.html#nearest-centroid-classifier>. Acesso em: 12 set. 2026.

[7] sklearn.metrics. Disponível em: <https://scikit-learn.org/stable/api/sklearn.metrics.html>. Acesso em: 12 set. 2026.

[8] SCIKIT-LEARN. 5.3. Preprocessing data — scikit-learn 0.21.3 documentation. Disponível em: <https://scikit-learn.org/stable/modules/preprocessing.html>. Acesso em: 12 set. 2026.

[9] DOS, Contribuidores. Distância euclidiana. Disponível em: <https://pt.wikipedia.org/wiki/Dist%C3%A2ncia_euclidiana>. Acesso em: 12 set. 2026.

[10] O que é a distância de Manhattan? Disponível em: <https://www.datacamp.com/pt/tutorial/manhattan-distance>. Acesso em: 12 set. 2026.

[11] Explicação da distância de Hamming: A teoria e os aplicativos. Disponível em: <https://www.datacamp.com/pt/tutorial/hamming-distance>. Acesso em: 12 set. 2026.

[12] Chebyshev distance. Disponível em: <https://en.wikipedia.org/wiki/Chebyshev_distance>. Acesso em: 12 set. 2026.

[13] CASSAR, Daniel R. ATP-203 1.1 - Tratamento de dados com pandas. 2026. Jupyter Notebook. Material didático não publicado.

[14] FILHO, Mario. Precisão, Recall e F1 Score Em Machine Learning. Disponível em: <https://mariofilho.com/precisao-recall-e-f1-score-em-machine-learning/>. Acesso em: 12 set. 2026.

[15] GEEKSFORGEEKS. AUC ROC Curve in Machine Learning. Disponível em: <https://www.geeksforgeeks.org/machine-learning/auc-roc-curve/>. Acesso em: 12 set. 2026.


## Docente responsável
| <img loading="lazy" src="https://github.com/user-attachments/assets/17dfa7bf-5ca9-42df-b63e-917827fc6308" width=115><br><sub> [Prof. Dr. Daneiel Roberto Cassar](http://lattes.cnpq.br/1717397276752482) |
| :--: |

## Desenvolvedora
| <img src="https://github.com/AnaLuizaSilv.png" width=115><br><sub>[Ana Luiza de Lima Silva](https://github.com/AnaLuizaSilv)</sub> |
| :--: |
Ana Luiza de Lima Silva, estudante do primeiro semestre do bacharelado em Ciência e Tecnologia da Ilum escola de ciência

<img width="966" height="95" alt="image" src="https://github.com/user-attachments/assets/f9825ded-4549-4691-a6e0-e261bfeb7aa1" />
