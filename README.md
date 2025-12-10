California Housing — Análise Estatística e Modelagem em Python

Este projeto tem como objetivo aplicar técnicas de Estatística, Aprendizado de Máquina e Análise Exploratória de Dados (EDA) utilizando o dataset California Housing, disponibilizado pela California Department of Housing and Community Development e distribuído via scikit-learn.

O trabalho segue o fluxo solicitado na disciplina, incluindo:

EDA completa

Regressão linear simples, múltipla e polinomial

Classificação (somente se aplicável, mas mantive estrutura)

Avaliação das métricas

Otimização dos modelos (GridSearchCV e PyCaret)

Discussão de limitações, vieses e próximos passos

1. Sobre o Dataset

O California Housing Dataset contém informações do censo de 1990 relativas a moradia no estado da Califórnia.

Variável-alvo

MedHouseVal – valor mediano das casas na região (em centenas de milhares de dólares).

Principais Features
Atributo	Descrição
MedInc	Renda média
HouseAge	Idade média das casas
AveRooms	Média de cômodos
AveBedrms	Média de quartos
Population	População
AveOccup	Ocupação média
Latitude	Latitude
Longitude	Longitude
Fonte

Distribuído por scikit-learn a partir do dataset original de
California Department of Housing and Community Development (1990).

Licença

Dataset disponível para uso educacional/pesquisa conforme redistribuição do scikit-learn.
2. Objetivos do Projeto

📌 O projeto tem como finalidade:

Realizar análise exploratória de dados (EDA)

Estatísticas descritivas

Tratamento de ausentes

Outliers

Correlação

Visualização (histogramas, boxplots, heatmap, pairplot)

Implementar modelos estatísticos e de machine learning:

Regressão Linear Simples

Regressão Linear Múltipla

Regressão Polinomial

(Opcional) Naive Bayes e Regressão Logística

Avaliar desempenho com métricas adequadas:

MAE

RMSE

R²

Análise de resíduos

Multicolinearidade (VIF)

Realizar otimização dos modelos:

Validação cruzada

GridSearchCV

PyCaret (compare_models / tune_model)

Produzir relatório com conclusões, limitações e próximos passos.

📊 3. Tecnologias Utilizadas
Categoria	Ferramenta
Manipulação de dados	pandas, numpy
Visualização	matplotlib, seaborn
Estatística	statsmodels
Machine Learning	scikit-learn, pycaret
Ambiente	Jupyter Notebook
5. Principais Resultados

👉 Regressão Linear Múltipla

R² entre 0.60 e 0.65

MedInc é a variável mais relevante

Presença moderada de heterocedasticidade

👉 Regressão Polinomial (grau 2)

Aumenta o R²

Maior custo computacional

Leve risco de overfitting

👉 PyCaret

Modelos como RandomForest e GradientBoosting apresentaram melhor desempenho

Tuning trouxe redução significativa de RMSE

⚠️ 6. Limitações e Vieses

Dados antigos (censo de 1990)

Variáveis geográficas limitadas

Possível multicolinearidade entre Latitude/Longitude

Ausência de variáveis econômicas ou sociais atuais

Dados agregados por região → perde granularidade

🔮 7. Próximos Passos

Aplicar modelos não lineares adicionais (XGBoost, CatBoost)

Criar mapas geoespaciais com Folium ou GeoPandas

Clusterização de regiões antes da regressão

Comparar com valores de mercado atuais

📝 8. Licença

Este projeto está licenciado sob a MIT License (ou escolha outra).
O dataset segue a licença de distribuição do scikit-learn.

👨‍💻 9. Autor

Fernando Otávio Bastos Oliveira
Projeto desenvolvido para a disciplina de Modelagem e Estatística / Machine Learning.
