# Comparação de Modelos de Classificação com o Dataset "Wine"

## Objetivo
Este projeto tem como objetivo treinar e avaliar três modelos de classificação usando o conjunto de dados "Wine" do `scikit-learn`. O foco é analisar o desempenho de cada modelo e identificar o mais eficaz para a classificação de vinhos com base em métricas como acurácia, precisão, recall e F1-score.

## Estrutura do Projeto
O projeto é dividido nos seguintes passos:
1. **Carregamento e Exploração do Dataset**:
   - Utilizamos o dataset `load_wine` do `scikit-learn`.
   - Exploramos as características (features) e o alvo (target) para entender as informações disponíveis.

2. **Pré-processamento dos Dados**:
   - Dividimos o dataset em treino (70%) e teste (30%).
   - Normalizamos as características para garantir que todas estejam na mesma escala, utilizando `StandardScaler`.

3. **Treinamento e Avaliação dos Modelos**:
   - Treinamos três modelos de classificação:
     - Árvore de Decisão
     - Random Forest
     - K-Nearest Neighbors (KNN)
   - Avaliamos cada modelo com as métricas:
     - Acurácia
     - Precisão
     - Recall
     - F1-score
   - Geramos a matriz de confusão para visualizar a performance em cada classe.

4. **Comparação dos Modelos**:
   - Comparação das métricas de cada modelo para identificar o que teve melhor desempenho.
   - Análise dos resultados e justificativas para a escolha do modelo com melhor performance.

## Relatório

i. Valores das Métricas para Cada Modelo
| Modelo               | Acurácia | Precisão | Recall | F1-Score |
|----------------------|----------|----------|--------|----------|
| **Árvore de Decisão**      | 0.96     | 0.96     | 0.96   | 0.96     |
| **Random Forest**          | 1.00     | 1.00     | 1.00   | 1.00     |
| **K-Nearest Neighbors**    | 0.96     | 0.97     | 0.96   | 0.96     |

ii. Modelo que se Destacou em Termos de Acurácia
O Random Forest teve a melhor acurácia, atingindo 1.00, o que indica que o modelo conseguiu classificar todas as amostras do conjunto de teste corretamente.

iii. Métrica mais Relevante para Decidir o Melhor Modelo
A métrica de F1-score foi a mais relevante nesta análise, pois considera tanto a precisão quanto o recall, fornecendo uma avaliação equilibrada entre a capacidade do modelo de evitar falsos positivos e falsos negativos. Como o Random Forest teve F1-score perfeito (1.00) em todas as classes, foi considerado o modelo com melhor desempenho.

iv. Modelo com Performance Significativamente Diferente
O Random Forest obteve um desempenho superior, especialmente por ter uma acurácia e F1-score perfeitos, ao contrário dos outros modelos que apresentaram pequenas quedas nessas métricas. Esse comportamento pode ser explicado pelo poder de ensemble do Random Forest, que combina várias árvores de decisão para aumentar a robustez e reduzir o risco de overfitting em comparação com uma única árvore de decisão.

Conclusão
i. Melhor Modelo para Este Conjunto de Dados
O Random Forest foi o modelo que apresentou o melhor desempenho para a classificação, alcançando 100% em acurácia e F1-score.

ii. Justificativa da Eficácia do Modelo Random Forest
O Random Forest foi eficaz devido à sua capacidade de combinar várias árvores de decisão, melhorando a generalização do modelo. Como o dataset Wine possui algumas classes bem representadas e um conjunto de features diversificado, o modelo conseguiu capturar bem as variações sem superestimar ruídos.

iii. Características dos Dados que Influenciaram o Desempenho
As características dos dados, como o equilíbrio relativo entre as classes e a presença de features informativas (como os níveis de flavonoides, álcool, etc.), contribuíram para que o Random Forest destacasse. O algoritmo soube explorar bem as combinações entre estas variáveis, especialmente por sua habilidade de reduzir o viés e variância combinando múltiplas árvores de decisão.