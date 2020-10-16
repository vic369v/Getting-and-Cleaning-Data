check if the data file is present in your working directory. (If not, will download and unzip the file)

Read data 
subject_test : subject IDs for test
subject_train : subject IDs for train
X_test : values of variables in test
X_train : values of variables in train
y_test : activity ID in test
y_train : activity ID in train
activity_labels : Description of activity IDs in y_test and y_train
features : description(label) of each variables in X_test and X_train
dataSet : bind of X_train and X_test

2. Extract only mean() and std()
MeanStdOnly : a vector of only mean and std labels 
dataSet : at the end of this step, dataSet will only contain mean and std variables

3. Changing Column label of dataSet
Create a vector of "clean" feature names by getting rid of "()" at the end
CleanFeatureNames : a vector of "clean" feature names

4. Adding Subject and Activity to the dataSet
subject : bind of subject_train and subject_test
activity : bind of y_train and y_test

5. Rename ID to activity name
act_group : factored activity column of dataSet

6. Output tidy data
baseData : melted tall and skinny dataSet
secondDataSet : casete baseData which has means of each variables
