## Step 1: Preprocess the Data

### Read in the charity_data.csv to a Pandas DataFrame

![2022-11-10 09_19_57-Window](https://user-images.githubusercontent.com/100164773/201116983-e6140f26-fe19-425c-a7b4-e997e22fd047.png)

### Drop unnecessary Data

![2022-11-10 09_20_16-Window](https://user-images.githubusercontent.com/100164773/201117063-3046b617-8d34-4e6f-a3b2-961396cda529.png)

### Determine the number of unique values for each column and reduce bigger unique sets.

![2022-11-10 09_29_02-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118274-d06c9238-317c-4248-9785-26308022cd51.png)

### Use bins to reduce number of sets to go through

![2022-11-10 09_29_12-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118295-d9f51aef-58f5-4301-af08-8a9a76fe1726.png)

![2022-11-10 09_29_20-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118327-0aa60fa6-46cd-4e94-9001-4c79fcf345b5.png)



![2022-11-10 09_30_53-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118588-850f23bf-367b-4804-9852-255e27ba37a6.png)

![2022-11-10 09_31_03-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118609-513eb332-4264-46a7-b371-dce2db539e8b.png)

### Use `pd.get_dummies()` to encode categorical variables.

![2022-11-10 09_32_57-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201118968-1e1dd90f-4ce7-42c0-b251-da3f5d2d5371.png)

<hr>

## Step 2: Compile, Train, and Evaluate the Model

### set up Nueral Network and created two hidden layers with an output layers

![2022-11-10 09_49_03-Starter_Code - Jupyter Notebook and 2 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201124189-318f3521-ed95-4ce9-b457-6f806bdc0c08.png)

### Then compiled and fit the data into the model 

![2022-11-10 14_24_11-Starter_Code - Jupyter Notebook and 3 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201187778-d5dda307-c86c-49f1-b49a-efa354398f37.png)

![2022-11-10 14_24_25-Starter_Code - Jupyter Notebook and 3 more pages - Personal - Microsoft​ Edge](https://user-images.githubusercontent.com/100164773/201187810-6f73cdd9-9df5-426b-944b-8af9ee2fd56b.png)

### Accuracy ended around .7335 with a loss of .565

<hr>

## Step 3: Optimize the Model

### Drop all rows where Special Conditions are equal to yes and Status is equal to 0

![2022-11-11 09_33_35-Window](https://user-images.githubusercontent.com/100164773/201362253-46935801-65f5-4cc9-bbc4-7b64cf5d88c9.png)

### Keep names and group all names that only appear once together

![2022-11-11 09_37_39-Window](https://user-images.githubusercontent.com/100164773/201362522-eeb5b23b-f870-4475-b1b9-439b1f0dab77.png)

### Make new smaller bins for Income Amount

![2022-11-11 09_37_51-Window](https://user-images.githubusercontent.com/100164773/201362544-9a4a8ee6-2f5e-4588-b9c8-991180686d3a.png)

### This will create fewer unique sets for the model to run through

![2022-11-11 09_38_01-Window](https://user-images.githubusercontent.com/100164773/201362564-00f5d4b9-5350-49ec-b6b2-eece181023f7.png)

![2022-11-11 09_40_25-Window](https://user-images.githubusercontent.com/100164773/201363000-9b6d04ab-a128-4a03-bbf5-549cac5579e6.png)

### Accuracy ended around .802 with a loss of .515

<hr>

## Step 4: Write a Report on the Neural Network Model

The purpose of our model is to predict the outcome of fundraisers depending on certain varibles. Those target varibles include Application Type, Affiliation Amount Asked for, Income Amount, and more. Ein number was removed from the set as it did not have any effect on the data set. 

The final amount of Layers were 6 hidden layers with 1 output layer and using the Relu function. These were found out by running . We passed our .75 goal with an accuracy of .802

With more testing we can drop the losses to lower than .5
