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

Machine and Deep learning para predição de crises financeiras

Assim, nossos esforços estiveram focados em transformar os dados brutos em indicadores que possam ser usados ​​para prever crises financeiras. Esses conjuntos de dados têm uma variável de resposta que indica se a instância país-ano teve uma crise ou não. Para antecipar as crises financeiras, o pré-processamento incluiu a criação de atributos econômicos que podem indicar uma crise, e também o indicador de resposta variável da crise foi antecipado dois anos antes de a crise realmente ocorrer. Além disso, períodos complicados da história foram removidos, como a crise financeira de 1929 e as duas grandes guerras do século passado.

Após o pré-processamento dos dados, focamos em remover o problema dos outliers: uma vez que temos poucas ocorrências de crise registradas, a variável resposta é desequilibrada. Portanto, usamos o método SMOTE para balancear nosso conjunto de dados e usamos o método Shuffle para embaralhar as novas instâncias.

Por fim, aplicamos os modelos preditivos: Regressão Logística (LogR), Máquina de Vetores de Suporte (SVM), Redes Neurais (NN), Florestas Aleatórias (RF) e Memória de curto prazo longa (LSTM).

Para obter os melhores parâmetros para construir esses modelos, usamos o método GridsearchCV para encontrá-los.

Finalmente, depois de explorar a busca por melhores parâmetros e criar outras propostas de conjuntos de dados, rodamos nossos modelos preditivos e usamos as métricas de acurácia, precisão, recall, pontuação F1 e curva ROC para observar os modelos vencedores.

Interpretamos que o modelo de RF, inicialmente usando o método de validação cruzada, obteve os melhores resultados e estamos confiantes de que nosso modelo pode ajudar em trabalhos futuros. Porém, ao utilizar a curva ROC, agora com o método train_test_split, os modelos RF e LSTM obtiveram resultados que devem ser considerados.

Todo esse projeto foi produzido na plataforma Google Collab em linguagem python.
