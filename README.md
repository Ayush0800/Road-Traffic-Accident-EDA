🚗 Road Traffic Accident Analysis
This project performs an Exploratory Data Analysis (EDA) on UK road traffic accident data. It involves data preprocessing, visualization, and detection of potential outliers in accident records to help derive meaningful insights.

📁 Dataset
The dataset is sourced from data.gov.uk, containing information about road accidents in the UK with features such as:

• Accident_Index

• Accident Date

• Number_of_Casualties

• Light_Conditions

• Weather_Conditions

• Accident_Severity


🛠️ Features Implemented
✅ Data Preprocessing
• Handled missing values by replacing empty strings with "No Data".

• Converted 'Number_of_Casualties' to integer type.

• Extracted year and month from the 'Accident Date'.

• Grouped all darkness-related entries into a single "Dark" category for better visualization.


📊 Data Visualization
• Pie charts for severity distribution and light condition impacts.

• Heatmaps for accident severity across various weather conditions.

• Line plots for monthly trends.

• Boxplots for identifying outliers in Number_of_Casualties.



📦 Boxplots for Outlier Detection
    Organized into a 2x2 grid:

• Number of Casualties

• Accident Severity vs Number of Casualties

• Light Conditions vs Number of Casualties

• Yearly Casualties Distribution



🚨 Outlier Detection
• Used the IQR (Interquartile Range) method to detect outliers in 'Number_of_Casualties'.

• Printed higher and lower outlier records in the console.

• Found that higher outliers were present, indicating potentially extreme accident cases.



📌 How to Run
  • Install required libraries:
```
bash
pip install pandas matplotlib seaborn
```
• Ensure your dataset CSV is named road-traffic-accidents.csv and placed in the same directory.

• Run the Python script:
```
bash
python traffic_analysis.py
```
📈 Sample Insights
• Most accidents happen under slight severity.

• Dark conditions contribute significantly to accident counts.

• Certain years show higher outlier activity.

• Weather conditions like rain and snow correlate with more casualties.



🧠 Future Scope
• Integrate machine learning to predict accident severity.

• Add interactive dashboards using Plotly or Dash.

• Explore geospatial analysis using location data.

👨‍💻 Author
Ayush Kumar
B.Tech CSE, Class of 2027
Exploring data-driven approaches to real-world safety.
