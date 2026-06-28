# AI Based Venturi Tube Design and CFD Performance Prediction Using Machine Learning

Predicting Venturi Tube CFD performance using Machine Learning models trained on ANSYS Fluent generated simulation data.

---

## Overview

This project explores the use of Machine Learning to predict the Computational Fluid Dynamics (CFD) performance of a Venturi tube without performing a new CFD simulation for every design.

A dataset containing **149 CFD simulation cases** was generated using **ANSYS Fluent Design of Experiments (DOE)**. The generated data was then used to train multiple machine learning regression models capable of predicting important flow parameters directly from Venturi tube geometry.

An additional inverse prediction model was also developed to recommend Venturi tube geometry based on desired CFD performance.

---

## Key Features

* Parametric Venturi tube design
* CFD dataset generation using ANSYS Fluent
* 149 Design of Experiments (DOE) simulation cases
* Forward prediction (Geometry → CFD)
* Inverse prediction (CFD → Geometry)
* Multi-output regression models
* Model performance comparison

---

## Technologies Used

* ANSYS Workbench
* ANSYS Fluent
* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Joblib

---

## Machine Learning Models

The following regression algorithms were implemented and compared:

* Random Forest Regressor
* Extra Trees Regressor
* Gradient Boosting Regressor

Performance was evaluated using:

* R² Score
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

---

## Dataset

**Inputs**

* Throat Length
* Diverging Length
* Converging Length
* Throat Diameter
* Inlet Diameter
* Outlet Diameter

**Outputs**

* Mass Flow Rate
* Inlet Pressure
* Outlet Pressure
* Maximum Velocity

Total CFD Cases: **149**

---

## Repository Structure

```text
Dataset/
Models/
Notebook/
Results/
Images/
README.md
```

---

## Future Improvements

* Increase CFD dataset size
* Improve prediction accuracy
* Hyperparameter optimization
* Integration with a desktop application
* Extension to other internal flow components

---
