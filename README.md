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
* <img width="477" height="445" alt="image" src="https://github.com/user-attachments/assets/c2646b59-0f84-4742-97ef-61a776d8717b" />


### Degree 3 (Cubic)

* Flexible enough to capture one bend/inflection.
* **Observation:** Tracks the main trend well without excessive oscillations.
* **Conclusion:**  **Good fit** – balanced errors, suitable complexity.
* <img width="433" height="442" alt="image" src="https://github.com/user-attachments/assets/b9b9bd38-a26d-4df9-8221-d1fa21a47ae8" />


### Degree 5 (Quintic)

* More flexible, can follow multiple bends.
* **Observation:** Captures details of the data but begins to show minor oscillations.
* **Conclusion:**  **Borderline – risk of overfitting**, especially if noise is present.
* <img width="411" height="439" alt="image" src="https://github.com/user-attachments/assets/1a50611d-52c2-4c1a-b162-5f86d34cc435" />


### Degree 6 (Sixth Order)

* Very flexible with many parameters.
* **Observation:** Fits training data very closely, but oscillates strongly and generalizes poorly.
* **Conclusion:**  **Overfitting** – low training error but high validation error.
* <img width="387" height="456" alt="image" src="https://github.com/user-attachments/assets/4963e2d6-a39f-486b-8261-7b24da79128c" />


---

## Key Takeaways

* **Low-degree models (1)** underfit the data.
* **Moderate-degree models (3)** often provide the best tradeoff.
* **High-degree models (5, 6)** risk overfitting, especially with noisy or limited data.

---



## License

This project is open for educational and research purposes.
