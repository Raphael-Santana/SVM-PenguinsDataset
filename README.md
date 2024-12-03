# Análise e Classificação dos Dados dos Pinguins 🐧

Este projeto realiza a análise e classificação dos dados de pinguins disponíveis no dataset do Seaborn. O objetivo é treinar e avaliar um modelo de classificação utilizando as características dos pinguins para prever seu sexo.

---

## Descrição do Projeto

O dataset dos pinguins contém informações sobre diferentes espécies de pinguins, incluindo características físicas como o tamanho do bico, massa corporal, entre outros. Neste projeto, utilizamos os dados para explorar e treinar um classificador SVM (`LinearSVC`) com as variáveis:

- `bill_depth_mm`: Profundidade do bico.
- `body_mass_g`: Massa corporal (em gramas).

O foco principal é prever o sexo dos pinguins (`male` ou `female`) com base nessas variáveis.

---

## Etapas Realizadas

1. **Importação e preparação dos dados**:
   - Carregamos o dataset diretamente do Seaborn, garantindo que os dados estão limpos e formatados.
   - Tratamos valores ausentes para evitar inconsistências.

2. **Divisão dos dados**:
   - Separação em conjunto de treino (70%) e teste (30%) utilizando `train_test_split` do `scikit-learn`.

3. **Treinamento do modelo**:
   - Treinamos um classificador `LinearSVC` com as variáveis `bill_depth_mm` e `body_mass_g`.
   - Visualizamos a fronteira (hiperplano) do modelo

4. **Avaliação do modelo**:
   - Relatório de classificação com precisão, recall e F1-score.
   - Matriz de confusão.
