# challenge--data-analysis
The aim of the project is learning.
Type of challenge:consolidation.
Duration:3 days.

Steps to do the project
1- open file by df=pd.read_csv('C:\\Users\\masrra\\Desktop\\data2.csv') 

2-Name the columns by using rename
df.rename(columns={'Column1':'property'},inplace=True)
df.rename(columns={'Column2':'Location'},inplace=True)
df.rename(columns={'Column3':'Price'},inplace=True)
df.rename(columns={'Column4':'Area'},inplace=True)
df.rename(columns={'Column5':'Number_of_Rooms'},inplace=True)
df.rename(columns={'Column6':'Furnished'},inplace=True)
df.rename(columns={'Column7':'Kitchen type'},inplace=True)
df.rename(columns={'Column8':'Status'},inplace=True)
df.rename(columns={'Column9':'Garden surface'},inplace=True)
df.rename(columns={'Column10':'Swimming Pool'},inplace=True)

3-classify property to house ,appartement and others.

4-Clean the property by using replace method or using for loop.

5-Clean number of rooms by extracting all letters from cells then use the condition to choose the required rooms number and in our project we need from 1 to 6 rooms.

6-Clean the price column by using (str.replace) to delete the (,) and (€)  

7-convert the string to numbers.

8-Make plot to the price column to see the result.

9-Clean the Garden Surface

Answer the questions in the project.
1-Which variable is the target ? the price of the property
2-How many rows and columns ? according to df.shape I have 9112 rows and 10columns
3-What is the correlation between the variables and the target ? (Why might that be?) I think the variables are the features 
that make us to predict the target
4-What is the correlation between the variables and the other variables ? (Why?)one of the variable considered as a features
and the others considered as a features
5-Which variables have the greatest influence on the target ?number of rooms,area,price
6-Which variables have the least influence on the target ?kitchen type,swimming pool,garden surface 
7-How many qualitative and quantitative variables are there ? How would you transform these values into numerical values ?
I transfer the value to numerical value by two ways,using astype(int) or pd.to_numeric().
quantity variables are number of rooms,price,area.
quality variables are property,status,swimming pool,furnished,location .
8-Percentage of missing values per column ?in my data there is no missing data or null data.
9-Are there any outliers? If yes, which ones and why?yes ,like number of rooms 400 .it is unlogic and it requires to clean it 
10- Which variables would you delete and why ?if you mean cells ,all the outlierss required to delete it 
and if you mean columns ,I think kitchen type,garden surface  
11-In your opinion, which 5 variables are the most important and why?the 5 most important values are price ,number of rooms
,location ,area,property.
12- In your opinion, which model of machine learning could solve the task of predicting the sales? Random forest according to google and multiple linear regression according to content
because I should use two features like number of rooms and property for example to predict the price (target)
