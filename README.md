Crop Prediction Using K-Nearest Neighbors (KNN)

This project predicts the most suitable crop based on soil and climate parameters using the K-Nearest Neighbors (KNN) classification algorithm.
The model compares three KNN distance metrics — Minkowski, Euclidean, and Manhattan — and automatically selects the method that produces the highest accuracy for final prediction.

🔧 Features

Accepts training dataset upload (.xlsx format)
Performs 80% training and 20% testing
Uses Elbow Method to determine the optimal value of K

Compares performance of:

Minkowski Distance
Euclidean Distance
Manhattan Distance

Automatically selects best-performing metric
Allows test dataset upload for prediction
Saves prediction results to Excel file (test_with_predictions.xlsx)

🧠 Input Requirements

Both training and test datasets must include the following columns:
Feature	Description:

N	           Nitrogen content
P	           Phosphorus content
K	           Potassium content
temperature	   Temperature (°C)
humidity	   Humidity (%)
ph	           Soil pH level
rainfall	   Rainfall (mm)

label	Crop name (only in training and optional in test data)

▶️ How to Run the Code

Run the notebook in Google Colab
Upload the training dataset when prompted

Observe:

Suggested optimal K
Accuracy of each KNN distance metric
Best metric selected automatically
Upload the test dataset
Download the generated test_with_predictions.xlsx file

📤 Output

Displays performance comparison of all 3 KNN methods
Clearly prints Best KNN Method and its accuracy
Adds a column Predicted to the test dataset
Saves the result to test_with_predictions.xlsx

📌 Notes

If the test file includes a label column, prediction accuracy is also shown.
If the label column is missing in the test file, predictions are still generated but comparison is skipped.

🏁 Summary

This implementation provides an enhanced KNN-based crop prediction system by:
Automatically tuning the optimal K
Comparing multiple distance metrics
Choosing the most accurate model for real-world prediction