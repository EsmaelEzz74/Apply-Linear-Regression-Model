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
