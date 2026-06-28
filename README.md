# AI-Based Venturi Tube Design and CFD Performance Prediction Using Machine Learning

> **Machine Learning framework for rapid prediction of Venturi tube CFD performance using ANSYS Fluent generated simulation data.**

---

## About the Project

Computational Fluid Dynamics (CFD) simulations are widely used to analyze Venturi tube performance, but they require significant computational time. This project demonstrates how Machine Learning can be used to accurately predict CFD results from Venturi tube geometry, eliminating the need to run a new CFD simulation for every design iteration.

A dataset of **149 CFD simulation cases** was generated using **ANSYS Fluent Design of Experiments (DOE)**. The generated dataset was used to train multiple machine learning regression models capable of predicting flow characteristics directly from geometric parameters.

The project also includes an inverse prediction model that recommends Venturi tube geometry for desired CFD performance.

---

## Project Highlights

* Parametric Venturi tube designed in ANSYS
* CFD simulations performed using ANSYS Fluent
* Dataset generated using Design of Experiments (DOE)
* 149 simulation cases used for model training
* Multi-output Machine Learning regression
* Forward Prediction (Geometry → CFD Outputs)
* Inverse Prediction (CFD Outputs → Geometry)
* Performance comparison of multiple ML algorithms

---

## Technologies Used

| Category            | Tools                         |
| ------------------- | ----------------------------- |
| CAD & Simulation    | ANSYS Workbench, ANSYS Fluent |
| Programming         | Python                        |
| Development         | Jupyter Notebook              |
| Data Processing     | Pandas, NumPy                 |
| Machine Learning    | Scikit-Learn                  |
| Visualization       | Matplotlib                    |
| Model Serialization | Joblib                        |

---

## Dataset

### Input Parameters

* Throat Length
* Diverging Length
* Converging Length
* Throat Diameter
* Inlet Diameter
* Outlet Diameter

### Output Parameters

* Mass Flow Rate
* Inlet Pressure
* Outlet Pressure
* Maximum Velocity

**Total CFD Simulation Cases:** **149**

---

## Machine Learning Models

The following regression models were developed and evaluated:

* Random Forest Regressor
* Extra Trees Regressor
* Gradient Boosting Regressor

### Evaluation Metrics

* R² Score
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

---

## Repository Structure

```
AI-Based-Venturi-Tube-Design-Using-Machine-Learning
│
├── Dataset/
│   └── venturi.xlsx
│
├── Notebook/
│   └── venturi.ipynb
│
├── Models/
│   ├── Forward_Model.pkl
│   ├── Inverse_Model.pkl
│   ├── ExtraTrees_Model.pkl
│   └── GradientBoosting_Model.pkl
│
├── Results/
│   └── Model_Comparison.xlsx
│
├── Images/
│
├── README.md
├── LICENSE
└── .gitignore
```

---

## Future Scope

* Expand the CFD dataset to improve model generalization.
* Optimize model performance using advanced hyperparameter tuning techniques.
* Integrate optimization algorithms for automated Venturi tube design.
* Extend the framework to other internal flow components.

---

## Author

**Harshita Yadav**

B.Tech in Mechanical Engineering

**Areas of Interest**

* Computational Fluid Dynamics (CFD)
* Machine Learning
* ANSYS Fluent
* Engineering Design
* Data-Driven Engineering
