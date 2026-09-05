# Delivery App Demand Predictor

A simple beginner-level machine learning project that helps delivery partners decide **which delivery app they should work with** based on the current situation.

The idea is simple:

When a delivery partner is going out to work, they may not know whether **Zomato, Swiggy, or Zepto** will have more delivery activity in a particular area and at a particular time.

This project uses basic data and a simple machine learning model to predict **which app is likely to have more traffic/delivery activity** based on a few conditions.

The goal is to help delivery partners make a better choice and potentially **maximize their earnings**.

## What the user enters

The model uses:

* **Area**
* **Time**
* **Weather**
* **Hard day**
* **Festival**

Based on these inputs, the model predicts one of:

* Zomato
* Swiggy
* Zepto

For example:

```text
Area: Jayanagar
Time: 19
Weather: Rainy
Hard day: Yes
Festival: No

Recommended app: Swiggy
```

The recommendation tells the delivery partner which platform is expected to have better delivery activity under those conditions.

## How it works

```text
User enters location + conditions
              ↓
        Data is prepared
              ↓
       Machine Learning Model
              ↓
     Predicts the best platform
              ↓
       Zomato / Swiggy / Zepto
```

The project is intentionally kept simple and beginner-friendly.

## Technologies Used

* Python
* Pandas
* Scikit-learn
* Jupyter Notebook
* Decision Tree Classifier

No APIs, databases, web applications, or complicated technologies are used.

## Project Structure

```text
delivery_app_traffic_predictor/
│
├── data.csv
├── delivery_app_traffic_predictor.ipynb
└── README.md
```

Everything is done inside the Jupyter Notebook.

## Machine Learning

A simple **Decision Tree Classifier** is used for prediction.

The notebook:

1. Loads the dataset using Pandas
2. Checks the size of the data
3. Looks at the available data
4. Selects the input features
5. Converts text values into numbers
6. Splits the data into training and testing data
7. Trains the Decision Tree
8. Checks the model accuracy
9. Takes user inputs through simple dropdowns
10. Predicts the recommended delivery platform

## Purpose of the Project

Delivery partners often work across multiple platforms and may have to decide where to spend their working hours.

Instead of choosing an app randomly, this project gives them a simple data-based prediction.

For example, depending on the **area, time, weather, and other conditions**, one platform may have more delivery activity than another.

The prediction can therefore help a delivery partner decide:

> **"Which app should I focus on right now if I want the best chance of maximizing my earnings?"**

This project is only a basic machine learning demonstration. It does **not** provide guaranteed earnings or live traffic information.

## Future Improvements

The project could later be improved by adding:

* Live delivery data
* Real-time demand
* Actual delivery earnings
* Distance between orders
* Number of available delivery partners
* Peak-hour information
* Historical earnings by area
* Live weather data

For now, the project focuses on understanding the basic machine learning workflow using a small dataset.
