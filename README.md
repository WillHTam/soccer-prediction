# soccer-prediction

- Attempt 1 yielded best of ~57% accuracy with KNN
- Attempt 2 yielded best of ~72% accuracy with LDA and Dense MLP

Conclusions:

- Data gathering and EDA take a long, long time

- Feature selection very important
  - For sports at least, better to take data points from events that have a relevant level of importance, ie predicting for the World Cup should use World Cup, European Championship, and other large tournament data instead of making trends noisy with friendlies where teams might not use their best squad / maximum ability etc.
  - Good feature selection outweighs parameter tuning

- Better to use raw data rather than complex transformations
  - Need to learn how to use grid_search for SVM better, and try different kernels

- Using more visualizations makes it easier to present to others
  - Also good to make clear sections of work (ie titled with Markdown) for your own and other's reference

- Using validation of different models is important in the event that 'better' models don't perform well

- Neural Network Notes
  - Data normalization is extremely important for NN's.  Adding SK Learn's StandardScaler instantly boosted results by 20% 
  - Excessive batch size does degrades model
  - Adam is not the end-all for optimizers, as it was outperformed here by RMSProp
  - ReLu however still outperforms all other activation functions tested


