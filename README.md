# Desenvolvimento de Modelo para Previsão de Consumo de Energia Elétrica Residencial

Neste projeto, meu objetivo foi prever o consumo residencial de energia no Brasil usando a metodologia CRISP-DM.

No pré-processamento utilizei técnicas como Winsorização para tratar outliers, criação de variáveis lagged (1 e 12 meses) para capturar tendências temporais, One-Hot Encoding (estado e mês) e transformação logarítmica (consumo) para preparar os dados para a modelagem.

Em seguida, fiz o teste e avaliação de diferentes algoritmos de regressão, incluindo Regressão Linear, Ridge, Lasso, ElasticNet, Árvore de Decisão, Random Forest e KNN, otimizando os hiperparâmetros com GridSearchCV e TimeSeriesSplit.
O modelo RandomForestRegressor obteve um ótimo desempenho, com R² de 0.995, RMSE: 0.060, MAE: 0.045 e MAPE: 41.84%.
