





| **Algoritmo** | **Tipo de Modelo** | **Princípio Principal** | **Vantagens** | **Desvantagens** | **Aplicações Típicas** |
| :-- | :-- | :-- | :-- | :-- | :-- |
| **Decision Tree** | Árvore simples | Divisão baseada em atributos | Interpretável, rápido | Overfitting, sensível a variações | Classificação, regressão básicas |
| **Random Forest** | Conjunto (bagging) | Múltiplas árvores com votação | Robustez, menos overfitting | Menos interpretável, mais lento | Classificação de grandes bases, bancos, seguros |
| **Gradient Boosting (GBM)** | Conjunto (boosting) | Árvores sequenciais ajustadas aos erros passados | Alta precisão, bom desempenho em competições | Mais lento, sensível a hiperparâmetros | Previsões complexas, competições Kaggle |
| **Support Vector Machine (SVM)** | Hiperplanos de margem | Maximize a margem entre classes | Funciona bem em alta dimensão, kernel | Necessita normalização, pode overfitar | Bioinformática, NLP, visão computacional |
| **k-Nearest Neighbors (kNN)** | Lazy learning | Baseado na proximidade dos vizinhos | Simples, eficiente com poucos atributos | Muito lento com grandes datasets, sensível ao escala | Classificação de pequenos datasets, recomendação |
| **Naive Bayes** | Probabilístico | Probabilidades condicionais | Rápido, bom com textos, simples | Assume independência, câmbio de distribuições | Filtragem de spam, análise de sentimentos |
| **Redes Neurais Artificiais** | Deep learning | Camadas de neurônios | Alta precisão, aprendizado profundo | Requer muitos dados, interpretabilidade reduzida | Reconhecimento facial, tradução automática |
| **XGBoost** | Gradient boosting otimizado | Árvore de decisão + boosting | Alta performance, popular em competições | Complexidade de ajuste | Previsão estruturada, ranking |
| **K-Means** | Clustering | Particionamento em k clusters | Simples, rápido | Difícil determinar k ideal, sensível a outliers | Segmentação de clientes, compressão de dados |
| **Hierarchical Clustering** | Clustering | Árvore de clusters | Visualização fácil, sincronia de agrupamentos | Computacionalmente intenso | Análise de plantas, segmentação de mercado |
| **Linear Regression** | Regressão | Ajuste linear simples | Intuitivo, rápido | Imóveis lineares, sensível a outliers | Previsões econômicas, previsão de vendas |
| **Lasso Regression** | Regularização | Regressão linear com penalidade | Seleção de variáveis, evita overfitting | Pode eliminar variáveis importantes | Previsão de risco, seleção de atributos |
| **Support Vector Regression (SVR)** | Regressão | Similar ao SVM | Funciona bem com dados não lineares | Necessita normalização, tuning de hiperparâmetros | Previsão de séries temporais |

### Observações importantes:

- **Normalização**: Algoritmos baseados em distâncias (como SVM, KNN, regressões) **necessitam** de normalização ou padronização dos dados para uma performance eficiente.
- **Árvores de decisão e ensemble**: Essas técnicas **não exigem** normalização, pois usam splits baseados em thresholds fixos de atributos, que preservam sua importância independente da escala.
