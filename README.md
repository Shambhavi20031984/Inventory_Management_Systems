# Inventory_Management_Systems
📘 Model Overview & Functionality – SMART_INVENT
The SMART_INVENT model is a machine learning-based inventory forecasting system tailored for restaurant and café businesses. It leverages an LSTM (Long Short-Term Memory) neural network to accurately predict future food demand based on historical order data. This time-series forecasting model is particularly suited for capturing trends and seasonality in customer behavior.
🧠 Model Architecture & Steps:
Data Preprocessing:

Loaded the historical food demand dataset.

Performed feature selection and handled missing/null values.

Normalized the data to ensure efficient LSTM training.

LSTM Model Implementation:

Built a sequential LSTM model with a hidden layer of 50 units.

Input shape: reshaped the training data into 3D for LSTM (samples, time steps, features).

Trained the model to learn patterns in daily/weekly demand.

Prediction & Evaluation:

Predicted demand on test data.

Visualized the comparison between predicted and actual demand using a dual-colored line graph (blue for actual, orange for predicted).

Used RMSE (Root Mean Squared Error) to assess prediction accuracy.

💰 Integration of Financial Equation:
To evaluate the financial implications of demand predictions, a simple but powerful financial equation was integrated:

𝑦
=
𝑚
⋅
𝑥
(
𝑡
)
−
𝐶
y=m⋅x(t)−C
​
 
Where:

𝑦
y: Total profit/revenue

𝑚
m: Selling price per unit

𝑥
(
𝑡
)
x(t): Predicted number of units sold at time 
𝑡
t

𝐶
C: Total production and maintenance cost

For example: If you sell a product at ₹1000, and the fixed cost 
𝐶
C is ₹1,00,000, then the profit becomes:

𝑦
=
1000
⋅
𝑥
(
𝑡
)
−
1
,
00
,
000
y=1000⋅x(t)−1,00,000
This transforms the LSTM-predicted demand into a financial forecast, enabling business owners to:

Estimate profits dynamically over time.

Make informed decisions on budgeting and inventory planning.

Forecast how market demand affects revenue and sustainability.

✅ Outcome:
The model successfully demonstrated the use of deep learning (LSTM) for demand forecasting and linked it to financial decision-making, creating a powerful tool for inventory and profit optimization in the food industry.

