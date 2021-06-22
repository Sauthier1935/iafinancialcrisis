# iafinancialcrisis
Machine and deep learning for predictiong financial crisis

We start from the identification of a dataset that is in the folders of this work. Afterwards, efforts were made to expand the amount of data, in the belief that more data, we can increase the precision and accuracy of our models. Thus, we have 4 datasets: boe (original, without data application), mean (which filled in missing cells with the average value of each country's attribute), median (which filled in missing cells with the median value of each country's attribute ) and most_f that filled missing cells with the most frequent value of each country's attribute.

Thus, our efforts were focused on transforming the raw data obtained in these datasets into indicators that can be used to forecast financial crises.
Such datasets have a response variable that indicates whether the country-year instance had a crisis. As we want to anticipate financial crises, our transformations, in addition to building economic attributes that may indicate crisis, the variable response indicator of crisis was brought forward to 2 years before the crisis actually occurred. Still, complicated periods of history have been removed, such as the financial crisis of 1929 and the two great wars of the last century.

After pre-processing these data, we focused on removing the outliers problem: since we have few registered occurrences of crises, the problem of financial crises ends up showing little in the response variable. Therefore, we use the SMOTE method to balance our dataset and we use the Shuffle method to shuffle the new instances.

Finally, we apply the predictive models: Logistic Regression (LogR), Support Vector Machine (SVM), Neural Networks (NN), Random Forests (RF) and Long short-term memory (LSTM).

To get the best parameters for building these models, we use the GridsearchCV method to find them.

Finally, after exploring the search for better parameters and creating other dataset proposals, we ran our predictive models and used the accuracy, precision, recall, F1-sccore and ROC curve metrics to observe the winning models.

We interpret that the RF model, initially using the cross-validation method, obtained the best results and we are confident that our model can help in future work. However, when using the ROC curve, now with the train_test_split method, the RF and LSTM models obtained results that should be considered.

Machine and Deep learning para predição de crises financeiras

Partimos desde a identificação de um dataset que está nas pastas deste trabalho. Após, realizados esforços para ampliar a quantidade de dados, na crença de que mais dados, podemos aumentar a precisão e acurácia dos nossos modelos. Sendo assim, temos 4 datasets: boe (original, sem apliação de dados), mean (que preencheu células faltantes com o valor médio do atributo de cada país), median (que preencheu células faltantes com o valor da mediana do atributo de cada país) e most_f que preencheu células faltantes com o valor mais frequente do atributo de cada país. 

Assim, nossos esforços foram concentrados em transformar os dados brutos obtidos nesses datasets em indicadores que podem ser utilizados para a previsão de crises financeiras.
Tais datasets possuem uma variável resposta que indica se a instância país-ano teve crise. Como queremos prevrer crises financeiras com atencedência, nossas transformações, além de construir atributos econômicos que podem indicar crise, a variável resposta indicadora de crise foi adiantada para 2 anos antes da crise de fato acontecer. Ainda, períodos complicados da história foram removidos, tais como a crise financeira de 1929 e as duas grandes guerras do século passado.

Após o pré processamento desses dados, nos concentramos em remover o problema de outliers: uma vez que temos poucas ocorrencias de crises registradas, o problema de crises financeiras acaba por aparecer pouco na variável resposta. Sendo assim, utilizamos o método SMOTE para balancear nosso dataset e utilizamos o método Shuffle para embaralhar as novas instâncias.

Finalmente, aplicamos os modelos preditivos: Regressão Logística (LogR), Support Vector Machine (SVM), Neural Networks (NN), Random Forests (RF) e Long short-term memory (LSTM).

Para obter os melhores parâmetros para a construção desses modelos, utilizamos o método GridsearchCV para encontrá-los.

Finalmente, após a exploração de busca de melhores parâmetros e criação de outras propostas de datasets, rodamos nossos modelos preditivos e utilizamos as métricas acurácia, precisão, recall, F1-sccore e curva ROC para observar os modelos vencedores.

Interpretamos que o modelo  RF, inicialmente utilizando o métdo de validação cruzada, obteve os melhores resultados e estamos confiantes que nosso modelo pode auxiliar em trabalhos futuros. No entanto, ao utilizar a curva ROC, agora com o método train_test_split, os modelos RF e LSTM obtiveram resultados que decem ser considerados.
