# Apply-Linear-Regression-Model-
Applying Linear Regression Model from SKlearn and from skratch

- For the auto-mpg data :
- First I read and load the data set with its column names
- I did some inspections to examine the data and its column types
- I use the pd.to_numeric function on the horsepower column to convert the object type to numeric 
- Then, by using the Seaborn library i draw a heatmap showing the correlation between the columns 
- <img src = "https://user-images.githubusercontent.com/85246622/207662320-5d16789d-f2f7-4eef-8a13-b03d9af7c527.png" width="400" height="400"/>
---------------------------------------------
- And with the seaborn's pair plot you can draw some types of plots like histogram 
- <img src = "https://user-images.githubusercontent.com/85246622/207663812-674d7afb-392b-49e8-be09-5b8a968127d6.png" width="600" height="400"/>
---------------------------------------------
- Then , I checked the data for null values and deleted 6 rows
- For my LR_Model function, which takes the data as X and Y as parameters :
- For 5 test size numbers I split the data into training and test sets 
- Then I fit X and Y using the linear regression model from Sklearn library below, I predict the y_test values and then compare them to the original y_test data to get the R2_score.
- Then for each test set, I print the test size and the R2_score and draw the scatterplot between the data in the two columns and the predicted line for the train and test data 
- <img src = "https://user-images.githubusercontent.com/85246622/207874340-f09d2840-a085-4431-a6e9-c8669ffed618.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207874389-ecba2ee7-5c36-4be0-999d-51288a340fab.png" width="400" height="400"/>
---------------------------------------------
- In my linear regression model, built from scratch, I First define a gradient_descent function that calculates the gradient descent by calculating the predicted y, cost function, the gradient, and then updating  the thetas to eventually get the best values for them to reach, I notice a breaking condition such that not all iterations are completed without reason 
- <img src = "https://user-images.githubusercontent.com/85246622/207876144-238ce5e9-581f-4690-b2de-575b976d0a8b.png" width="600" height="300"/>
---------------------------------------------
- In the LR_model function, I entered a fixed test size of 0.2 and split the data using train_test_split Then I used MinMaxScaler to perform data normalization
- Then using the above gradient descent funtion I predict the data and get the hypothesis the get the R2_score
- Next, I print the R2_score,  I draw the number of graphs that help to understand the evaluation of the model as follows: 
- Draws a graph between the cost function and the number of iterations 
- Draw a graph between the cost function and the updated thetas_0 list
- Draw a graph between the cost function and the updated thetas_1 list
- Draw a scatterplot between the data in the two columns and any predicted outputs 
- Finally, a scatterplot between the data in the two columns and the line that best fits the data
---------------------------------------------
- Finally, I tested my function on three columns and printed the results as follows :
- Dicplacement column :
- <img src = "https://user-images.githubusercontent.com/85246622/207883496-21f33eca-99a8-46ec-aff3-f18a6d168d7c.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207883556-48fe7072-bd96-47a7-b061-ab322559d904.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207883669-557e3d5a-21c7-4ef0-bd21-979d1f252b01.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207887052-7346f85c-f46d-4134-8f20-ede7b838ba74.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207887102-528eb2c8-9cc0-42cd-9901-6e8557db3cce.png" width="400" height="400"/>
---------------------------------------------
- Horsepower column :
- <img src = "https://user-images.githubusercontent.com/85246622/207884372-d446866d-ef25-4124-bb0d-0e512421f008.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207884453-fcf0e4a9-e0a6-4d5f-ae35-7a46f17e5af9.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207884539-4ffa4d4f-8590-499d-8f52-963251ea96ab.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207886871-8bb1fde7-d804-47f0-8ccd-fc817c0d360a.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207886937-239897dd-9a3b-4e24-9a02-4ac5e0da7e92.png" width="400" height="400"/>
---------------------------------------------
- Weight column :
- <img src = "https://user-images.githubusercontent.com/85246622/207885377-1e7ec170-c2b6-4d12-9919-fa56d22af8ec.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207885437-ed3addfc-e9f6-4bd0-abae-12f72b4e57ac.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207885520-3a3a7b50-1d68-4e85-b278-a33c393fa96e.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207887249-8657e630-1e36-4e9b-8e95-2fce74a5e8bf.png" width="400" height="400"/> <img src = "https://user-images.githubusercontent.com/85246622/207887305-f3c9151b-d7d8-4192-ae07-b9635d546a04.png" width="400" height="400"/>
