
# Discrete Choice Analysis

In this exercise, we will apply the multinomial logistic model to individual-level discrete choice data. The goal is to learn how to format the data, apply the R package "mlogit" to fit a multinomial logistic model and interpret the results. 

The setting of the exercise is about consumers' choices of shopping malls. In this dataset, each of the 500 consumers from a same city chooses a shopping mall to visit every week in 12 weeks. There are 4 different shopping malls and a consumer also has the option of choosing not to visit any of them in a week. Hence, the choice set is denoted as {"1", "2", "3", "4", "0"}, where 1 through 4 are the ID's of the 4 malls and 0 means not visiting any of them (often called the outside option in a choice model).  The columns in the dataset are as follows.  

customer ID:	The ID of the customer
mode:	 This represents the choice alternatives for a consumer 
choice:	A binary dummy variable that marks which alternative in the choice set is chosen
Week:	A weekly time period indicator 
discount:	An index which shows the level of discounts offer at the mall; a greater number means higher discount
targeting:	Whether a consumer receives a targeting message from the shopping mall in that week {1 = Yes, 0 = No}
distance:	The distance between a consumer's home to the shopping malls 
income:	The income level of the customer
gender:	Gender indicator {1 = Male, 0 = Female}
