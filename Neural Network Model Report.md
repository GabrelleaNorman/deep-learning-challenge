
# Deep Learning Challenge: Predicting Charity Funding Success

## Summary

Alphabet Soup, a non-profit foundation, endeavors to develop an algorithm employing machine learning and neural networks to predict the success of funding applicants. The goal is to create a binary classifier capable of determining whether applicants will succeed if funded by Alphabet Soup.

## Data Processing

- The initial step involved removing irrelevant information, such as EIN and NAME.
- The remaining columns were considered as features for the model, with NAME reintroduced in the second test for binning purposes.
- The dataset was divided into training and testing sets.
- The target variable, labeled "IS_SUCCESSFUL," was assigned values of 1 for yes and 0 for no.
- Analysis of the APPLICATION data involved binning the "CLASSIFICATION" values, with a cutoff for rare variables, grouping them under a new category, "Other."
- Categorical variables were encoded using the `get_dummies()` function after confirming successful binning.

## Model Compilation, Training, and Evaluation

- Each model, post Neural Network application, comprised three layers.
- The number of hidden nodes was determined by the number of features, resulting in a three-layer model with 6461 parameters.
- The initial accuracy was slightly below the desired 75% at  73%.
- Subsequent optimization, including the inclusion of the "NAME" column, led to an accuracy of nearly 79%, surpassing the target by 4%.
- This improved accuracy was achieved with 3,298 parameters.
![Screenshot 2023-11-13 211613](https://github.com/GabrelleaNorman/deep-learning-challenge/assets/130908954/dbd107e1-33b7-4a32-a24e-8194237d5c32)
![Screenshot 2023-11-13 212749](https://github.com/GabrelleaNorman/deep-learning-challenge/assets/130908954/8e5224c3-cd86-4f37-bb96-5fbb4945b85e)
![Screenshot 2023-11-13 212708](https://github.com/GabrelleaNorman/deep-learning-challenge/assets/130908954/8823e5bb-e0c8-4981-af2b-f263d52c7437)
![Screenshot 2023-11-13 212940](https://github.com/GabrelleaNorman/deep-learning-challenge/assets/130908954/9a28a0aa-3ea3-4be2-8604-d58acca08726)

## Optimization Insight

- The decision to incorporate multiple layers in the deep learning models aligns with the idea that such architectures enhance the model's ability to predict and classify information.
- Deep learning involves the systematic filtering of inputs through layers, allowing the model to learn intricate patterns and relationships within the data.

In summary, a Random Forest model could be a pragmatic alternative, offering good predictive performance, interpretability, and robustness for the charity funding prediction problem, especially in scenarios where the dataset is moderate in size and the relationships are not excessively complex.
