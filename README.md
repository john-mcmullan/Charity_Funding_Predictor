### Step 1: Preprocess the Data

Read in the charity_data.csv to a Pandas DataFrame

![2022-11-10 09_19_57-Window](https://user-images.githubusercontent.com/100164773/201116983-e6140f26-fe19-425c-a7b4-e997e22fd047.png)

Drop unnecessary Data

![2022-11-10 09_20_16-Window](https://user-images.githubusercontent.com/100164773/201117063-3046b617-8d34-4e6f-a3b2-961396cda529.png)

Determine the number of unique values for each column and reduce bigger unique sets.

![2022-11-10 09_29_02-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118274-d06c9238-317c-4248-9785-26308022cd51.png)

![2022-11-10 09_29_12-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118295-d9f51aef-58f5-4301-af08-8a9a76fe1726.png)

![2022-11-10 09_29_20-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118327-0aa60fa6-46cd-4e94-9001-4c79fcf345b5.png)

C:\Users\johnm\OneDrive\Documents\SA Images\2022-11-10 09_31_25-Editing Charity_Funding_Predictor_README.md at main · john-mcmullan_Charity_Fund.png

![2022-11-10 09_30_53-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118588-850f23bf-367b-4804-9852-255e27ba37a6.png)

![2022-11-10 09_31_03-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118609-513eb332-4264-46a7-b371-dce2db539e8b.png)

Use `pd.get_dummies()` to encode categorical variables.

![2022-11-10 09_32_57-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118968-1e1dd90f-4ce7-42c0-b251-da3f5d2d5371.png)
<hr>
### Step 2: Compile, Train, and Evaluate the Model

set up Nueral Network and created two hidden layers with an output layers

![2022-11-10 09_49_03-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201124189-318f3521-ed95-4ce9-b457-6f806bdc0c08.png)

Then compiled and fit the data into the model 

![2022-11-10 14_24_11-Starter_Code - Jupyter Notebook and 3 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201187778-d5dda307-c86c-49f1-b49a-efa354398f37.png)

![2022-11-10 14_24_25-Starter_Code - Jupyter Notebook and 3 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201187810-6f73cdd9-9df5-426b-944b-8af9ee2fd56b.png)

Accuracy ended around .7335 with a loss of .565
<hr>
### Step 3: Optimize the Model

Using your knowledge of TensorFlow, optimize your model to achieve a target predictive accuracy higher than 75%.

Using any or all of the following methods to optimize your model:

* Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
  * Dropping more or fewer columns.
  * Creating more bins for rare occurrences in columns.
  * Increasing or decreasing the number of values for each bin.
* Add more neurons to a hidden layer.
* Add more hidden layers.
* Use different activation functions for the hidden layers.
* Add or reduce the number of epochs to the training regimen.

**Note**: If you make at least three attempts at optimizing your model, you will not lose points if your model does not achieve target performance.

1. Create a new Jupyter Notebook file and name it `AlphabetSoupCharity_Optimzation.ipynb`.

2. Import your dependencies and read in the `charity_data.csv` to a Pandas DataFrame.

3. Preprocess the dataset like you did in Step 1, Be sure to adjust for any modifications that came out of optimizing the model.

4. Design a neural network model, and be sure to adjust for modifications that will optimize the model to achieve higher than 75% accuracy.

5. Save and export your results to an HDF5 file. Name the file `AlphabetSoupCharity_Optimization.h5`.
<hr>
### Step 4: Write a Report on the Neural Network Model

The purpose of our model is to predict the outcome of fundraisers depending on certain varibles. Those target varibles include Application Type, Affiliation Amount Asked for, Income Amount, and more. Ein number and the Name were removed from the set as they will not have an effect on the data set. 

The final amount of neurons were _____ with _____ layers and _______ activation functions. These were run by running aa search through the model to determine the most optimal set up. We were just short of our .75 accuracy goal with a score of .74.

Overall results of .74 accuracy with ______ losses show we can do more to optimize. Grouping of Ask amount would be the next big step to take.
