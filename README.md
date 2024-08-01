# Selecting Location for an Oil Well

Steps for selecting a location:

- Search for deposits in the selected region, determine the values ​​of the attributes for each;
- Build a model and estimate the volume of reserves;
- Select deposits with the highest estimated values. The number of deposits depends on the company's budget and the cost of developing one well;
- Profit is equal to the total profit of the selected deposits.


## **Introduction:**

### *Project Description:*
  
    We will study oil samples in three regions provided by the company.
    We will build a model to determine the region where oil production will bring greater profit.
    
### *Project Goal:*
    Select a location for wells that will bring greater profit and less loss.
### *Data Description:*
    Data in three tables: geo_data_0, geo_data_1, geo_data_2:
      id — unique well identifier;
      f0, f1, f2 — three point attributes;
      product — volume of reserves in the well (thousand barrels);
### *Work Plan:*
    1. Loading data, studying general information.
    2. Data preprocessing: check for abnormal values, gaps, duplicates, data types
    3. Exploratory data analysis: study important patterns and draw conclusions about the necessary data preparation.
    4. Data preparation: we will prepare the features in the pipeline.
    5. Training and testing the model for each region:
      5.1. Split the data into training and validation sets in a ratio of 75:25.
      5.2. Train the model and make predictions on the validation set.
      5.3. Save the predictions and correct answers on the validation set.
      5.4. Print the average stock of the predicted raw materials and the RMSE of the model on the screen.
      5.5. Analyze the results.
    6. Preparation for profit calculation:
      6.1. Save all key values ​​for calculations in separate variables.
      6.2. Calculate a sufficient volume of raw materials for break-even development of a new well. Compare the resulting volume of raw materials with the average stock in
    each region.
      6.3. Write conclusions on the stage of preparation for profit calculation.
    7. Calculating risks and profits for each region.
      7.1 Write a function to calculate profit for selected wells and model predictions
      7.2 Apply Bootstrap technique with 1000 samples to find profit distribution
      7.3 Find average profit, 95% confidence interval and risk of loss
    8. General conclusion
