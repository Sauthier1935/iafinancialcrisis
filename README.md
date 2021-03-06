# iafinancialcrisis
Machine and Deep Learning for Predicting Financial Crises

We start with the identification of a dataset that is in the folders of this work. Afterward, efforts were made to expand the amount of data, in the belief that with more data, we can increase the precision and accuracy of our models. Thus, we have 4 datasets: boe (original, without missing data treatment), mean (missing data filled with the average value of each country's attribute), median (missing data filled with the median value of each country's attribute ), and most_f (missing data filled that with the most frequent value of each country's attribute). All these methods of filling in to extend the dataset are obtained from the SimpleImputer technique.

Thus, our efforts were focused on transforming the raw data into indicators that can be used to forecast financial crises. Such datasets have a response variable that indicates whether the country-year instance had a crisis or not. In order to anticipate financial crises, the pre-processing included the creation of economic attributes that may indicate a crisis, and also the variable response indicator of the crisis was brought forward two years before the crisis actually occurred. In addition, complicated periods of history have been removed, such as the financial crisis of 1929 and the two great wars of the last century.

After data pre-processing, we focused on removing the outliers problem: once we have few registered crisis occurrences, the response variable is unbalanced. Therefore, we use the SMOTE method to balance our dataset and we use the Shuffle method to shuffle the new instances.

Finally, we apply the predictive models: Logistic Regression (LogR), Support Vector Machine (SVM), Neural Networks (NN), Random Forests (RF) and Long short-term memory (LSTM).

To get the best parameters for building these models, we use the GridsearchCV method to find them.

Finally, after exploring the search for better parameters and creating other dataset proposals, we ran our predictive models and used the accuracy, precision, recall, F1-score, and ROC curve metrics to observe the winning models.

We interpret that the RF model, initially using the cross-validation method, obtained the best results and we are confident that our model can help in future work. However, when using the ROC curve, now with the train_test_split method, the RF and LSTM models obtained results that should be considered.

This entire project was produced on the Google Collab platform in python language.

Machine and Deep learning para predi????o de crises financeiras

Come??amos com a identifica????o de um conjunto de dados que est?? nas pastas deste trabalho. Posteriormente, esfor??os foram feitos para ampliar a quantidade de dados, na cren??a de que com mais dados podemos aumentar a precis??o e exatid??o de nossos modelos. Assim, temos 4 conjuntos de dados: boe (original, sem tratamento de dados ausentes), m??dia (dados ausentes preenchidos com o valor m??dio do atributo de cada pa??s), mediana (dados ausentes preenchidos com o valor mediano do atributo de cada pa??s) e most_f ( dados ausentes preenchidos com o valor mais frequente do atributo de cada pa??s). Todos esses m??todos de preenchimento para estender o conjunto de dados s??o obtidos a partir da t??cnica SimpleImputer.

Assim, nossos esfor??os estiveram focados em transformar os dados brutos em indicadores que possam ser usados ??????para prever crises financeiras. Esses conjuntos de dados t??m uma vari??vel de resposta que indica se a inst??ncia pa??s-ano teve uma crise ou n??o. Para responder ??s crises financeiras, o pr??-processamento incluiu a cria????o de atributos econ??micos que podem indicar a crise, e tamb??m os indicadores vari??veis ??????da crise foram antecipados dois anos antes da efectiva. Al??m disso, per??odos complicados da hist??ria foram removidos, como a crise financeira de 1929 e as duas grandes guerras do s??culo passado.

Ap??s o pr??-processamento dos dados, nos concentramos em remover o problema dos outliers: uma vez registradas as ocorr??ncias de crise, a vari??vel resposta fica desequilibrada. Portanto, usamos o m??todo SMOTE para balancear nosso conjunto de dados e usamos o m??todo Shuffle para embaralhar as novas inst??ncias.

Por fim, aplicamos os modelos preditivos: Regress??o Log??stica (LogR), M??quina de Vetores de Suporte (SVM), Redes Neurais (NN), Florestas Aleat??rias (RF) e Mem??ria de curto prazo longa (LSTM).

Para obter os melhores par??metros para construir esses modelos, usamos o m??todo GridsearchCV para encontr??-los.

Finalmente, depois de explorar a busca por melhores par??metros e criar outras propostas de conjuntos de dados, rodamos nossos modelos preditivos e usamos as m??tricas de acur??cia, precis??o, recall, pontua????o F1 e curva ROC para observar os modelos vencedores.

Interpretamos que o modelo de RF, inicialmente usando o m??todo de valida????o cruzada, obteve os melhores resultados e estamos confiantes de que nosso modelo pode ajudar em trabalhos futuros. Por??m, ao utilizar a curva ROC, agora com o m??todo train_test_split, os modelos RF e LSTM obtiveram resultados que devem ser considerados.

Todo esse projeto foi produzido na plataforma Google Collab em linguagem python.
