# iafinancialcrisis
Machine and deep learning for predictiong financial crisis

We start from the identification of a dataset that is in the folders of this work. Afterwards, efforts were made to expand the amount of data, in the belief that more data, we can increase the precision and accuracy of our models. Thus, our efforts were focused on transforming the raw data obtained into indicators that can be used to forecast financial crises. Our dataset has a response variable that indicates whether the country-year instance had a crisis. As we want to prevent financial crises, our dataset transformations, in addition to building attributes that may indicate crisis, the crisis response variable was brought forward to 2 years before the crisis actually occurred. Still, complicated periods of history have been removed, such as the financial crisis of 1929 and the two great wars of the last century.

After the creation of the dataset, we removed the outliers problem: since we have few registered crisis occurrences, the financial crisis problem ends up showing little in the response variable. Therefore, we use the SMOTE method to balance our dataset and we use the Shuffle method to shuffle the new instances.

Finally, we apply the predictive models: Logistic Regression (LogR), Support Vector Machine (SVM), Neural Networks (NN), Random Forests (RF) and Long short-term memory (LSTM).

To obtain the best parameters for building these models, we use the GridsearchCV method to find them.

Finally, after exploring the search for better parameters and creating other dataset proposals, we ran our predictive models and used the accuracy, precision, recall, F1-sccore and ROC curve metrics to observe the winning models.

We interpret that the RF model, initially using the cross-validation method, obtained the best results and we are confident that our model can help in future work. However, when using the ROC curve, now with the train_test_split method, the RF and LSTM models obtained results that should be considered.

Machine and Deep learning para predição de crises financeiras

Partimos desde a identificação de um dataset que está nas pastas deste trabalho. Após, realizados esforços para ampliar a quantidade de dados, na crença de que mais dados, podemos aumentar a precisão e acurácia dos nossos modelos. Assim, nossos esforços foram concentrados em transformar os dados brutos obtidos em indicadores que podem ser utilizados para a previsão de crises financeiras. Nosso dataset possui uma variável resposta que indica se a instância país-ano teve crise. Como queremos prevrer crises financeiras, nossas transformações no dataset, além de construir atributos que podem indicar crise, a variável resposta indicadora de crise foi adiantada para 2 anos antes da crise de fato acontecer. Ainda, perídos complicados da história foram removidos, tais como a crise financeira de 1929 e as duas grandes guerras do século passado.

Após a criação do dataset, removemos o problema de outliers: uma vez que temos poucas ocorrencias de crises registradas, o problema de crises financeiras acaba por aparecer pouco na variável resposta. Sendo assim, utilizamos o método SMOTE para balancear nosso dataset e utilizamos o método Shuffle para embaralhar as novas instâncias.

Finalmente, aplicamos os modelos preditivos: Regressão Logística (LogR), Support Vector Machine (SVM), Neural Networks (NN), Random Forests (RF) e Long short-term memory (LSTM).

Para obter os melhores parametros para a construção desses modelos, utilizamos o método GridsearchCV para encontrá-los.

Finalmente, após a exploração de busca de melhores parâmetros e criação de outras propostas de datasets, rodamos nossos modelos preditivos e utilizamos as métricas acurácia, precisão, recall, F1-sccore e curva ROC para observar os modelos vencedores.

Interpretamos que o modelo  RF, inicialmente utilizando o métdo de validação cruzada, obteve os melhores resultados e estamos confiantes que nosso modelo pode auxiliar em trabalhos futuros. No entanto, ao utilizar a curva ROC, agora com o método train_test_split, os modelos RF e LSTM obtiveram resultados que decem ser considerados.
