# Spam_classification

Classificação de SPAM

O SMS Spam Collection é um conjunto de mensagens SMS marcadas que foram coletadas para a pesquisa de SMS Spam. Ele contém um conjunto de mensagens SMS em inglês de 5.574 mensagens, marcadas como ham (legítimo) ou spam.

O conjunto de dados original pode ser encontrado em https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection. 

A questão para usar esse banco de dados, como conta no Kagglw é: Você pode usar esse conjunto de dados para construir um modelo de previsão que classifique com precisão quais textos são spam? 

Referência:
Almeida, T.A., Gómez Hidalgo, J.M., Yamakami, A. Contributions to the Study of SMS Spam Filtering: New Collection and Results. Proceedings of the 2011 ACM Symposium on Document Engineering (DOCENG'11), Mountain View, CA, EUA, 2011.

SOLUÇÃO PROPOSTA e RESULTADOS

Para resolver esse problema de NLP foi construído uma classificação usando Machine Learning em python. A IDE Visual Studio Code foi usada para a Análise de Dados e Machine Learning, atravês dos seguintes pacotes: Pandas, Scikit-learn, Scipy e Spacy.

Utilizamos um modelo de Decision Tree, Random Forest e uma Baseline Dummy, econtrando os seguintes resultados, respectivamente:


    Accuracy com dummy stratified, 10 = [86.43, 86.75]

    Accuracy médio 95.93
    Intervalo [95.17, 96.68]

    Accuracy médio 95.62
    Intervalo [93.75, 97.49]


Os modelos com esses melhores resultados, foram:


    DecisionTreeClassifier(max_depth=30, min_samples_leaf=2, min_samples_split=16)

    RandomForestClassifier(bootstrap=False, criterion='entropy', max_depth=40,
                       min_samples_leaf=2, min_samples_split=8,
                       n_estimators=10)




CONCLUSÃO

Através desse projeto foi possível praticar e implementar conceitos importantes da Ciência de Dados e propor uma solução para um problema um problema de Classificação.
