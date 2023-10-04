## Concrete Compressive Strength Prediction

*Dataset :* [link](https://www.kaggle.com/maajdl/yeh-concret-data)

## Overview:
- Concrete is the most important material in civil/structural engineering.
- The compressive strength of concrete is significantly influenced by both age and ingredients in a nonlinear manner.
- The problem is to develop a regression model for predicting concrete compressive strength using various features from training data, considering different raw material contents, mixture optimization for cost-effectiveness, and maximizing strength based on available material quantities.

### Data Information:

The provided information includes variable names, types, measurement units, and brief descriptions. This dataset focuses on predicting concrete compressive strength, making it a regression problem. The order of the variables aligns with the sequence of numbers in the database rows.

| Name                  | Data Type | Measurement          | Description                  |
|-----------------------|-----------|----------------------|------------------------------|
| Cement (component 1)  | Quantitative | kg in a m3 mixture | Input Variable              |
| Blast Furnace Slag (component 2) | Quantitative | kg in a m3 mixture | Input Variable |
| Fly Ash (component 3) | Quantitative | kg in a m3 mixture | Input Variable |
| Water (component 4)   | Quantitative | kg in a m3 mixture | Input Variable              |
| Superplasticizer (component 5) | Quantitative | kg in a m3 mixture | Input Variable |
| Coarse Aggregate (component 6) | Quantitative | kg in a m3 mixture | Input Variable |
| Fine Aggregate (component 7)   | Quantitative | kg in a m3 mixture | Input Variable |
| Age                   | Quantitative | Day (1~365)          | Input Variable              |
| Concrete Compressive Strength | Quantitative | MPa(mega pascal)               | Output Variable             |

### Takeaways from EDA and Feature Engineering:

- Cement, water, coarse aggregate, and fine aggregate could exhibit a normal distribution following appropriate transformations.
- Transformations might reveal a bi-modal distribution in the slag and fly ash columns.
- The Superplasticizer column distinctly conforms to a tweedie distribution.
- The Age column can be discretized into bins and then transformed into a categorical feature.
- Outliers treatment required.
- Overall data is little bit right skewed. 
- The data needs to be standardized.
- Both the above requirements can be met by a feature transformation.
