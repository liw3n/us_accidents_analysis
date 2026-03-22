# Programming for Big Data Group Project
## Dataset
[US Accidents on Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents/data)
### Overview
There are two notebook files, namely 'traditional_US_accidents_analysis.ipynb' and 'pyspark_US_accidents_analysis.ipynb', along with the datasets 'US_Accidents_March23.csv' and 'historical_state_population_by_year.csv'. There is also a smaller sample dataset if you would like to use this when assessing the traditional implementation 'US_Accidents_March23_sampled_500k.csv'.

Each notebook is split into 5 tasks completed by each group member.

### Instructions for Traditional Solution 
1. Please ensure the datasets are in the same working directory as the notebook files. 
2. For the traditional solultion, you should run 'traditional_US_accidents_analysis.ipynb'.

### Instructions for Optimal Solution
This notebook 'pyspark_US_accidents_analysis.ipynb' should be run using openJDK version 17.0.18, apache-spark 4.1.1, and anaconda python 3.13.9, on an M1 Pro Apple Macbook Pro with 16gb of RAM. Please ensure your device can give up to 8GB of RAM to this notebook for execution purposes.
1. Please ensure the datasets are in the same working directory as the notebook file 'pyspark_US_accidents_analysis.ipynb'
2. There is an optional cell to configure Java path for openJDK 17, and python.
3. Next, ensure you for the spark session find '.config("spark.driver.memory", "8g")', if your device cannot allocate this program 8GB then please try 6g or 4g.
4. Once ready execute each cell.

Note that this notebook has been tested and runs without error with 8g allocated memory for spark session, along with openJDK version 17, apache-spark 4.1.1 and Python version 3.13.9.

### Notes
We find for some tasks the Spark implementation has a slower execution time than the traditional implementation. This can be seen for the POI analysis. This is likely due to overhead when implementing Spark. However for more complex operations such as loading and cleaning the data, along with the in-depth weather analysis, the Spark implementation is considerably faster than the traditional implementation.
