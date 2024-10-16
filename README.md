# Atividade Titanic

## Etapas do Projeto
1. Carregamento dos Dados: A base de dados do Titanic foi importada.
2. Tratamento de Dados Faltantes: Valores ausentes foram preenchidos utilizando a mediana para a idade e a moda para o porto de embarque. Registros com valores ausentes na coluna 'Cabin' foram excluídos.
3. Seleção de Atributos: Foram escolhidas as colunas relevantes para a análise: Pclass, Sex, Age, Fare e Survived. A coluna Sex foi convertida em variáveis dummy para facilitar a análise.
4. Divisão dos Dados: Os dados foram separados em conjuntos de treino (70%) e teste (30%).
5. Treinamento do Modelo: Um modelo k-NN foi treinado utilizando k=3.
6. Avaliação do Modelo: O desempenho do modelo foi avaliado com base na acurácia, relatório de classificação e matriz de confusão.
etapa

## Acurácia

A acurácia do modelo foi de X.XX, indicando a porcentagem de previsões corretas em relação ao total de previsões realizadas.

## Relatório de Classificação

O relatório de classificação apresenta métricas como precisão, recall e F1-score. A precisão indica a proporção de verdadeiros positivos em relação ao total de positivos previstos, enquanto o recall mede a capacidade do modelo de identificar todos os verdadeiros positivos.

## Matriz de Confusão

A matriz de confusão fornece uma visão detalhada das previsões do modelo. Os valores na matriz representam:

- Verdadeiros Negativos (TN): Passageiros que não sobreviveram e foram corretamente classificados.
- Falsos Positivos (FP): Passageiros que não sobreviveram, mas foram incorretamente classificados como sobreviventes.
- Falsos Negativos (FN): Passageiros que sobreviveram, mas foram incorretamente classificados como não sobreviventes.
- Verdadeiros Positivos (TP): Passageiros que sobreviveram e foram corretamente classificados.

Matriz de Confusão: [[TN FP] [FN TP]]

## Análise e Melhorias

- Testar Diferentes Valores de "k": O valor de k pode ter um impacto significativo no desempenho do modelo. É recomendável realizar uma validação cruzada para determinar o valor ideal de k.
- Explorar Mais Características: A inclusão de variáveis adicionais e relevantes pode ajudar a melhorar a precisão do modelo.
- Ajustar os Parâmetros do Modelo: Realizar uma busca em grade para otimizar os hiperparâmetros do k-NN pode levar a um melhor desempenho do modelo.