# Polynomial Regression Fit Analysis



[Open the Colab Notebook](https://colab.research.google.com/drive/16AJRkqCnEdjG7IykTtKtcqJdzWXbzGFA?usp=sharing)

---

## Objective

The goal is to study **underfitting, good fitting, and overfitting** behavior by fitting polynomials of degree 1, 3, 5, and 6 to the dataset and visually/quantitatively comparing their performance.

---

## Steps Performed

1. Loaded the dataset into Colab.
2. Split the data into **training** and **validation** sets.
3. Fitted polynomial regression models with degrees **1, 3, 5, and 6**.
4. Calculated **training error** and **validation error** for each degree.
5. Plotted the fitted curves against the actual data to observe model behavior.

---

## Results & Interpretation

### Degree 1 (Linear)

* Produces a straight-line fit.
* **Observation:** Cannot capture curvature in the data.
* **Conclusion:**  **Underfitting** – high training/validation error.

### Degree 3 (Cubic)

* Flexible enough to capture one bend/inflection.
* **Observation:** Tracks the main trend well without excessive oscillations.
* **Conclusion:**  **Good fit** – balanced errors, suitable complexity.

### Degree 5 (Quintic)

* More flexible, can follow multiple bends.
* **Observation:** Captures details of the data but begins to show minor oscillations.
* **Conclusion:**  **Borderline – risk of overfitting**, especially if noise is present.

### Degree 6 (Sixth Order)

* Very flexible with many parameters.
* **Observation:** Fits training data very closely, but oscillates strongly and generalizes poorly.
* **Conclusion:**  **Overfitting** – low training error but high validation error.

---

## Key Takeaways

* **Low-degree models (1)** underfit the data.
* **Moderate-degree models (3)** often provide the best tradeoff.
* **High-degree models (5, 6)** risk overfitting, especially with noisy or limited data.

---



## License

This project is open for educational and research purposes.
