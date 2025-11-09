# Rainfall Prediction in Australia

This project explores weather data from Australia with the goal of predicting whether it will rain the next day. The idea is simple and practical: if we can make this prediction, we can help support decisions in agriculture, transportation, city planning, and even daily life (like deciding whether to bring an umbrella).

The dataset used includes daily weather observations such as temperature, humidity, pressure, and wind conditions collected across multiple locations in Australia.

---

##  Goal of the Project
The main objective was to build a machine learning model that can answer a **binary question**:

 **Will it rain tomorrow?**  
> **Yes**  or **No** 

To do this, we:
- Explored and cleaned the data
- Built and trained prediction models
- Compared two models to see which performed better:
  - **Random Forest Classifier**
  - **Logistic Regression**

---

## Models Used

### 1. **Random Forest Classifier**
- Performed well at overall prediction.
- Strong at recognizing patterns from multiple weather features.
- However, it struggled a bit to correctly identify the *rainy days* (true positives).

### 2. **Logistic Regression**
- A simpler, more interpretable model.
- Performed similarly in overall accuracy.
- Also had challenges predicting "Yes" (rain) cases, but behaved more consistently.

---

## Results Summary

| Model | Accuracy (overall) | Approx. Correct Predictions | True Positive Rate (Correctly predicting Rain) |
|------|-------------------|----------------------------|------------------------------------------------|
| **Random Forest** | ~84% | ~1270 correct predictions | ~50% correctly predicted rain |
| **Logistic Regression** | ~83% | ~1255 correct predictions | ~51% correctly predicted rain |

**Takeaway:**  
Both models are good at predicting "no rain" days, which are more common in the dataset. However, both still have room to improve at detecting rainy days — which is the more difficult and important part of the prediction task.

---

## What I Learned
- How to clean and prepare real-world weather data
- How to train and evaluate machine learning classification models
- The importance of comparing different models, not just choosing one
- How imbalance in real data affects predictions (predicting rare events is harder)

---

## Next Steps (How This Could Be Improved)
To improve performance, especially for detecting rainy days, I could:
- Use **class balancing techniques** to give more weight to the rain class
- Try **additional models** like Gradient Boosting or XGBoost
- Engineer new features (e.g., humidity differences between morning and evening)
- Fine-tune hyperparameters more deeply

---

## Technologies Used
- **Python**
- **Pandas & NumPy**
- **Scikit-learn**
- **Matplotlib / Seaborn**
- **Jupyter Notebook**

---

## Final Thoughts
Weather prediction is challenging, and this project was a clear example of how **data tells a story**, but also how important it is to choose the right tools and modeling strategy. Even simple models can perform well if the data is prepared thoughtfully.

If you'd like to explore or contribute, feel free to fork the project!


