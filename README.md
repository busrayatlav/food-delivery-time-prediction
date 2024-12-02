# Food Delivery Time Prediction

## Overview
This project predicts the food delivery time based on factors such as:
- Age and ratings of the delivery partner.
- Distance between the restaurant and delivery location.
- The dataset includes real-world features such as coordinates, vehicle type, and order type.

Using Python and LSTM neural networks, the project models delivery times to help food delivery services optimize their operations.

---

## Dataset
The dataset contains the following features:
- **Delivery_person_Age**: Age of the delivery partner.
- **Delivery_person_Ratings**: Average ratings from previous deliveries.
- **Restaurant_latitude & longitude**: Coordinates of the restaurant.
- **Delivery_location_latitude & longitude**: Coordinates of the delivery location.
- **Type_of_order**: Type of food ordered (e.g., Snack, Drinks, Buffet).
- **Type_of_vehicle**: Vehicle used by the delivery partner.
- **Time_taken(min)**: Time taken for delivery (target variable).

### Source
The dataset is provided for educational purposes and contains over 45,000 data points.

---

## Installation

### Step 1: Clone the Repository
```
git clone https://github.com/yourusername/food-delivery-time-prediction.git
cd food-delivery-time-prediction
```
### Step 2: Install Dependencies
Install the required Python libraries:
```
pip install -r requirements.txt
```

---

## Project Workflow

### 1. Data Preprocessing
- Calculated the distance between restaurant and delivery location using the **Haversine formula**.
- Cleaned the data and ensured no null values.

### 2. Exploratory Data Analysis (EDA)
- Visualized relationships between:
  - Distance and delivery time.
  - Age, ratings, and delivery time.
  - Vehicle type, order type, and delivery time.

### 3. Model Training
- Used **LSTM neural networks** to train a model on:
  - Delivery partner's age and ratings.
  - Calculated distance.

### 4. Predictions
- Predicted delivery time in minutes based on input features:
  - Delivery partner's age.
  - Average ratings.
  - Total distance.

---

## Usage

### Running the Project
1. Open the terminal in the project directory.
2. Run the script to train the model and make predictions:
   ```
   python food_delivery_time_prediction.py
   ```
3. ### 3. Example Input:

- **Age of Delivery Partner**: 29  
- **Ratings of Previous Deliveries**: 4.5  
- **Total Distance**: 6  

### 4. Example Output:
- **Predicted Delivery Time in Minutes**: 28  

---

## Results

- The **LSTM Neural Network** effectively models food delivery times.
- Features contributing most to delivery time:
  - Delivery partner's age.
  - Ratings from previous deliveries.
  - Distance between the restaurant and delivery location.

---

## Dependencies

- Python 3.7+
- Pandas
- NumPy
- Plotly
- Scikit-learn
- TensorFlow/Keras

---

## Future Improvements

- Include weather and traffic conditions for better predictions.
- Add real-time tracking for dynamic updates.
- Deploy the project as an interactive web application using **Streamlit** or **Flask**.

---

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions or improvements.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgements

- **Dataset**: Provided for educational purposes.
- **Inspiration**: Inspired by Aman Kharwal's article on food delivery time prediction.
- **Libraries and Tools**: Built using Python, Pandas, TensorFlow, and Plotly.

---

## Repository Structure

```
food-delivery-time-prediction/

│

├── food_delivery_time_prediction.py   # Main Python script

├── deliverytime.txt                   # Dataset file

├── requirements.txt                   # List of required libraries

├── README.md                          # Project documentation

└── LICENSE                            # License file

```


