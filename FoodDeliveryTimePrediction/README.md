# ML-Projects
# 🚴‍♂️ Food Delivery Time Prediction 🕒

This project focuses on predicting the time taken by food delivery agents to deliver an order based on various factors like the delivery distance, type of order, vehicle type, and ratings of the delivery person. The objective is to build a machine learning model that accurately estimates the delivery time to enhance the customer experience and improve logistics.

---

## 📂 Dataset Description

The dataset used is a cleaned version of a publicly available dataset from Kaggle (originally submitted by Gaurav Malik). The features included are:

| Feature Name                | Description                                                  |
|----------------------------|--------------------------------------------------------------|
| ID                         | Unique Order ID                                              |
| Delivery_person_ID         | ID of the delivery agent                                     |
| Delivery_person_Age        | Age of the delivery person                                   |
| Delivery_person_Ratings    | Average ratings of the delivery partner                      |
| Restaurant_latitude        | Latitude of the restaurant                                   |
| Restaurant_longitude       | Longitude of the restaurant                                  |
| Delivery_location_latitude | Latitude of the customer's location                          |
| Delivery_location_longitude| Longitude of the customer's location                         |
| Type_of_order              | Type of meal (e.g., Meal, Snack, Drinks, Buffet)             |
| Type_of_vehicle            | Type of vehicle used for delivery                            |
| Time_taken(min)            | Target variable — time taken for delivery (in minutes)       |

---

## ✅ Objective

> Predict the delivery time (`Time_taken(min)`) of food orders based on input features using a regression model.

---

## 💡 Project Workflow

1. **Import Libraries & Load Dataset**
2. **Basic Data Exploration & Cleaning**
3. **Feature Engineering**
   - Distance Calculation using Haversine Formula
   - Encoding Categorical Variables
4. **Model Building**
   - Train-Test Split
   - Model Training (Linear Regression)
5. **Model Evaluation**
6. **Visualization**
7. **Result Summary**

---

## 🛠️ Tools & Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📊 Distance Feature Engineering

We calculate the distance between the restaurant and delivery location using the **Haversine Formula**, which accounts for the curvature of the Earth:

```python
def haversine(lat1, lon1, lat2, lon2):
    ...

