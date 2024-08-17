# Meta-Aprendizado com Algoritmos de Machine Learning

Este repositório contém um estudo sobre meta-aprendizado usando sete algoritmos de machine learning: Regressão Logística, Árvore de Decisão, Floresta Aleatória, KNN, SVM, Naive Bayes, Gradient Boosting, e Perceptron. Realizei quatro testes distintos para avaliar o desempenho desses algoritmos em diferentes cenários, com o objetivo de identificar o mais adequado para cada tipo de problema.

## Testes Realizados

### 1. Verificação do Melhor Algoritmo com Validação Cruzada (5-Fold)
No primeiro teste, utilizei uma validação cruzada de 5 divisões (fold) para avaliar a acurácia dos algoritmos. O destaque foi o algoritmo **Floresta Aleatória**, que obteve uma pontuação de 0.94.

### 2. Meta-Aprendizado com 10.000 Amostras
Para o segundo teste, apliquei meta-aprendizado em um conjunto de 10.000 amostras, com 12 características e 4 classes. Aqui, usei grupos aleatórios de 0 a 9 para a validação cruzada. Mais uma vez, **Floresta Aleatória** se destacou, com uma acurácia de 0.90.

### 3. Teste com 30 Características e 2 Classes
No terceiro teste, aumentei o número de características para 30, mantendo 2 classes e validando com grupos aleatórios de 0 a 8. O melhor resultado foi alcançado pelo **Gradiente Boosting**, com uma acurácia média de 0.93.

### 4. Verificação do Menor Tempo de Treinamento
O último teste focou em identificar o algoritmo com o menor tempo de treinamento, usando validação cruzada de 5 divisões (fold) e avaliando a acurácia. O **Naive Bayes** foi o mais rápido, com um tempo de treinamento de 0.05 segundos e uma acurácia de 0.88.

## Análise dos Algoritmos

### Regressão Logística
A Regressão Logística não se destaca em bases de dados com muitos atributos irrelevantes devido à sua dependência de relações lineares entre as características. Ela funciona bem para dados numéricos e categóricos com boas relações lineares. Um exemplo prático é a classificação de e-mails como spam ou não.

### Árvore de Decisão
As Árvores de Decisão são sensíveis a pequenas variações nos dados, o que pode resultar em saídas diferentes com facilidade. São adequadas para dados categóricos e numéricos onde a interpretabilidade é crucial, como na análise de risco em decisões financeiras.

### Floresta Aleatória
Apesar de sua complexidade e tempo de treinamento elevado, a Floresta Aleatória é ideal para bases de dados com alta dimensionalidade e correlação entre características. Apresenta bons resultados em problemas de detecção de fraudes, classificação de imagens, e previsão de crédito.

### K-Vizinhos Mais Próximos (KNN)
O KNN é ineficiente em grandes conjuntos de dados e sensível a características irrelevantes e à normalização. É mais adequado para dados numéricos bem distribuídos e de baixa dimensionalidade, sendo útil em reconhecimento de padrões e sistemas de recomendação.

### Support Vector Machine (SVM)
O SVM possui um alto custo computacional, tornando-o ineficiente para grandes conjuntos de dados, especialmente aqueles com ruídos ou sobreposição entre classes. É ideal para dados numéricos com fronteiras de decisão claras, como na detecção de anomalias.

### Naive Bayes
O Naive Bayes assume independência entre características, o que pode ser problemático quando essa suposição é violada. É mais eficaz com dados categóricos, como em análise de sentimentos em redes sociais.

### Gradiente Boosting
Embora robusto, o Gradiente Boosting é propenso a overfitting e requer mais tempo de treinamento. É adequado para bases de dados complexas com interações não lineares, sendo utilizado em previsões de risco de crédito e ações.

### Perceptron
O Perceptron é limitado a problemas linearmente separáveis e é incapaz de aprender padrões complexos ou não lineares. Funciona bem com dados numéricos binários ou escalados, como na classificação de imagens binárias.

## Conclusão
A escolha do algoritmo mais adequado depende das características específicas dos dados e do problema a ser resolvido. Neste estudo, a **Floresta Aleatória** demonstrou um desempenho superior em termos de acurácia na maioria dos testes. No entanto, é essencial considerar o tempo de treinamento e a complexidade dos dados ao selecionar o algoritmo mais adequado para cada aplicação.
