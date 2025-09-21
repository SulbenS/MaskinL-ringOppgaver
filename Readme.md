# Required libraries


```
pip install scikit
pip install pandas
pip install kagglehub
pip install matplotlib
pip install scikit-learn
pip install seaborn
```

# Evaluation

## Knowledge to make an evaluation

- RMSE (Root Mean Squared Error): Measures the average magnitude of the prediction error. The lower the RMSE, the better the performance
- R^2 (Coefficient of determination): Measures how well the model explains the variance in the target variable. The close to 1 the better.

## Analysis
- The Ensamble model achived the lowest RMSE and highest R^2, indicating it has the most accurate predictions and explains the most variance in the target variable. This indicates this is the most suited model for this task.
- The Polynomial model improved the Linear model, having a lower RMSE and increased R^2
- The Linear model had the worst result, showing it is less fit for analysing the data in the Ames Hosuing dataset.

## Conclusion
For the training dataset we have worked with, the model that yielded the best accuracy was the RandomForestEnsamble.

# Feature Selection

## Implemented
- Most people do not look at the square footage of different floors, but rather the property as a whole, so we added that.
- The total amount of bathrooms is something most people are interested in knowing.
- Some people are more interested in how much are they have for their porch.
- Most people only care if the is a fireplace, garage or pool, not usually the size of that area itself.

## Other features we think would be important, but were missing
- Location of the house (impact on price can vary)
- Total amount of bedrooms in the house (simular to the bathrooms this would be useful for price prediction)
- Population 