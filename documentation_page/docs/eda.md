# Welcome to my capstone project "Credit Risk Assessment"

## Exploratory data analysis

The data that I used for this project is loan data of around 32000 borrowers that contains 12 columns including the target variable “loan status”. In the exploratory data analysis I analyzed the data, searched for patterns and prepared the data for training. 



## Outliers

The data had some outliers in various features like

* person employment lenght which contained a max of 123 years 
* person income which contained a max of 6.000.000 $ with a median of 55.000 $ 
* person age which contained a max of 144 years

After some further exploration of these outliers I deleted the rows containing these values. 


## NaN Values

The data had two features that contained some NaN values. 

* There were 895 rows with NaN values in the column person employment length. I imputed these missing values with the median value for all employment length.
* There were 3116 rows with NaN values in the column loan interest rate. I deleted the rows with missing values in this column. 

	        
## Distribution

In credit risk assessment it is common to deal with data that is highly imbalanced regarding the target class. This is because usually there are more people that pay back their loan than people that do not pay back their loan. In the used dataset there are about 3.58 times more non defaults than defaults. In the final model training I am therefore using different methods to optimize for imbalanced data.