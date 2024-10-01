# Cinema Ticket Sales Prediction

This project builds a predictive model to forecast cinema ticket sales using the **Cinema Tickets dataset**, which includes sales history and screening details from various cinemas over eight months in 2018.

## Code Steps

1. **Data Preprocessing**:
   - Drop irrelevant column (`date`) from the features.
   - Using (`total_sales`) as the target.
   - Handle missing data by filling with zeros.
   
2. **Modeling**:
   - A **Linear Regression** model is trained to predict ticket sales.

3. **Evaluation**:
   - The model's performance is assessed using **Mean Squared Error (MSE)**.
