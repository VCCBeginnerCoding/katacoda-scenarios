# Trainer Notes for Week 4:
This document is to help you lead the Week 4 session. This week's content is more hands on and practical so make sure you are familiar with the content and the code should a participant ask you questions regarding the content. 

I would also recommend just trying the course yourself as you'll pick up problems along the way. By doing so, you'll be more prepared for any questions participants might have. 

## Subtopic 1: Pandas
Pandas is a software library written for Python for data manipulation and analysis. In particular it offers data structures and operations for manipulating and analysing 'Dataframes' which are essentially tables.  

To install pandas we must run the command "python3 -m pip install pandas"

To import the library we run "import pandas" 

The following code block shows how to read spreadsheets and csv into python via pandas. If xlsx doesn't work , it's due to the katacoda VM not supporting the .xlsx format. Running this code in your windows machine will work. 

### Your turn! : Pandas
Get the participants to try and load the file "data.csv" into the variable "data_df" using the technique seen in the above code block. 

The following line prints out the data frame to show the participants what the data has. 

The data contains random expenditure data. It contains the CAPEX and OPEX data as well as the total amount.  


## Subtopic 2: Processing data in Pandas
In this subtopic, the idea is for the participants to discover what some key functions in pandas do. There are 4 functions, head, tail, describe and value counts. 

Possible ideas; 
1. Go through each function 1 by 1 and encourage discussion amongst the group. What does the function do?
2. Get them to write all them at once and then go through each function and discuss what the function does

It is important that the participants think about where this functionality would be useful and how they might use it in a data analysis environment. 

This is also important to get the participants to understand the data. Ask them questions about what the data is. The data is fake financial data CAPEX (capital expenditure), 
OPEX (operational expenditure) and Total Expenditure (CAPEX + OPEX). 

After the participants have written all the functions, they should have a better idea with what our data shows.


## Subtopic 2: Visualizing data in Pandas
In this subtopic, we are exploring the different types of visualization graphs pandas has built in. In the example I use line graph and box plot however you can go into other graphs should you find it to be useful during the session. The complete list of options can be found here : https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.html 


There is also a question, "What is the most suitable type of graph for the example data?". This is posed as a question to get participants thinking in an analytical way. Understanding visualization and how best to present is a key aspect of data science. 


## Subtopic 3: Data Analysis in Pandas
In this subtopic we are digging into the main aspect of pandas - data analysis. 

There are many "Your Turn" blocks in this section with all of them following the example code above. It is important that the participants aren't just copying the above code, but they are thinking of what they are doing and that they understand why they are doing what they are doing.


## Subtopic 4: Mini Project
In this subtopic we are revising all the concepts used above in one mini project. 

The idea of this mini project is the challenge the participants. If the participants get stuck tell them to refer to code above first and if they still don't understand to come to you for help. 

If participants don't manage to finish the mini project take it away for homework , try complete it in the free time. For those that do manage to finish the mini project, there are extension topics which involve filtering and processing. The extension is designed to challenge the participants and to ask questions about their data. 

The data in this project is taken from Kaggle and is a dataset of people's age, education level, income and how much wine they buy. 









