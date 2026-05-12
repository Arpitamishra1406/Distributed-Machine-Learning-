# Distributed-Machine-Learning-
💻 Banking Data Analysis with Apache Spark – Data Parallelism Project
📌 Project Objective

This project shows how Apache Spark can handle and analyze large banking datasets using parallel processing. The dataset (bank.csv) contains customer information collected during bank marketing campaigns for term deposit subscriptions.

🗂️ About the Dataset

The dataset includes details such as:

Client age
Job type
Marital status
Education level
Account balance
Housing loan and personal loan status
Contact details
Campaign information
Previous marketing outcomes
Subscription result (y)
⚙️ Tools & Technologies Used
Apache Spark
PySpark (Spark SQL & MLlib)
Python
Google Colab
🚀 Work Done in the Project
1️⃣ Data Loading & Partitioning
Loaded the bank.csv dataset into Spark DataFrame.
Used repartition() on the job column to improve parallel processing speed.
2️⃣ Parallel Data Analysis
Calculated average account balance for different job categories using groupBy() and avg().
Created age groups and identified which age category had the highest number of personal loans.
📊 Main Finding
People between 30–39 years had the highest number of personal loans.
Retired and student clients showed higher average balances.
3️⃣ Machine Learning with Spark ML

Built a Logistic Regression model to predict whether a client will subscribe to a term deposit.

Steps Followed
Split data into training and testing sets.
Converted categorical columns using StringIndexer.
Combined features using VectorAssembler.
Trained the model using Spark MLlib.
4️⃣ Model Evaluation

The model performance was checked using:

Accuracy
Precision
Recall
F1 Score
📈 Result

The Logistic Regression model performed well and successfully predicted customer subscriptions using distributed processing.

5️⃣ Resource Monitoring
Used the psutil library to monitor CPU and memory usage.
Observed higher CPU usage during Spark parallel execution while memory usage stayed efficient.
6️⃣ Task Scheduling in Spark
Spark’s DAG Scheduler automatically managed task execution.
Lazy evaluation helped optimize processing and improve performance.
📂 FILE 2 – Machine Learning with Spark ML
🧠 Term Deposit Subscription Prediction

This project focuses on predicting whether a customer will subscribe to a term deposit using Spark MLlib.

🎯 Objective
Preprocess banking data
Train a machine learning model
Evaluate performance
Improve results using hyperparameter tuning
🔄 Workflow
✅ Data Preprocessing
Loaded and checked dataset
Converted categorical data into numeric format
Prepared features for model training
✅ Model Training
Used Logistic Regression
Training Data: 80%
Testing Data: 20%
✅ Evaluation Results
Accuracy: 89.17%
Precision: 87.07%
Recall: 89.17%
F1 Score: 87.07%
✅ Hyperparameter Tuning

Applied:

ParamGridBuilder
CrossValidator
📊 Important Features
poutcome strongly affected prediction results.
Housing loans had a positive effect.
Personal loans negatively affected subscriptions.
📂 FILE 3 – Spark Data Processing Project
💳 Bank Client Data Analysis using Spark
🎯 Objective

To analyze banking customer data using Spark and generate useful business insights.

📌 Tasks Performed
✅ Data Inspection
Loaded dataset
Checked schema and summary statistics
✅ Filtering & Transformations
Filtered clients with balance greater than 1000
Added quarter column based on month
✅ Aggregation
Average balance by job type
Count of subscribed clients by marital status
✅ UDF Implementation

Created custom age groups:

Below 30
30–60
Above 60
✅ Advanced Analysis
Subscription rate by education level
Default rates by profession
✅ Visualization

Used:

Pandas
Matplotlib

Created:

Bar charts
Pie charts
📊 Important Insights
Older clients had higher balances.
Management was the most common job type.
Cellular contact method gave better campaign success.
Credit default cases were very low.
FILE 4 – Real-Time Machine Learning with Spark Streaming
🔄 Real-Time Banking Analysis using Spark Streaming
📌 Project Overview

This project simulates live banking transaction analysis using Spark Structured Streaming.

✅ Tasks Completed
1️⃣ Streaming Data Processing
Split bank.csv into chunks
Simulated real-time streaming input
Calculated live average balances and durations
2️⃣ Real-Time Predictions
Trained a machine learning model using historical data
Used the model to generate live predictions on streaming data
3️⃣ Window Operations

Analyzed trends using:

10-second windows
1-minute windows
4️⃣ Handling Late Data
Applied watermarking
Managed delayed and out-of-order records efficiently
🛠️ Technologies Used
Spark Structured Streaming
PySpark
Python
Google Colab
📂 FILE 5 – Banking Data Analysis using Pandas
💼 Hadoop & Hive Project (Implemented using Pandas)
📌 Objective

This project analyzes banking customer data using Pandas instead of Hadoop and Hive for easier implementation in Google Colab.

✅ Analysis Performed
Average balance by job
Housing loan analysis
Monthly campaign trends
Correlation between age and balance
Subscription analysis
Top clients by account balance
Education-level insights
📊 Key Findings
Retired and management clients had higher balances.
May recorded the highest number of client contacts.
Previous successful campaigns increased subscription chances.
Age and balance showed weak correlation.
🛠️ Technologies Used
Python
Pandas
Google Colab
Matplotlib
✅ Final Conclusion

These projects demonstrate how Apache Spark and related tools can efficiently process and analyze large-scale banking datasets. Using Spark’s distributed processing, machine learning, and streaming capabilities, meaningful business insights and prediction models were successfully developed for banking marketing campaigns.
