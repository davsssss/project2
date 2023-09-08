# project2

Crowdfunding Extract, Transform, Load

## Background: 
In this assignment, we were tasked with creating 4 total CSV files after creating dataframes of information provided to us in excel format. The CSV files were then used to draw an ERD diagram and two SQL schema files that are saved in our project files. We split the assignment into two parts between us. Below is our process and results are within our repository. 

## Category And Subcategory DataFrames: 

David: I started by creating the 'category' and 'subcategory' dataframes. To complete this I started by splitting the 'category & subcategory' column from the crowdfunding.xlsx into individual lists and getting the unique values. I then created unique ID's for each given category and subcategory using list comprehension. I then created a category dataframe using the category_id and category list (same for subcategory). Then I created the campaign dataframe by using the required columns from the crowdfunding.xlsx. After getting the required columns changed the 'goal' and 'pledged' datatypes to float along with changing the names and datatypes of the 'launched_at' and 'deadline' columns. All created dataframes were saved to their own .csv. All instructions came from project 2 in module 13.

## Contacts DataFrame

William: I was tasked with utilizing the contacts.xlsx file in our resources folder to create a contacts dataframe within pandas and output my dataframe to a CSV file. In order to do this I started by reading in the data from the excel file. I needed to utilize header=3 instead of the instructed header=2 due to the position of contact_info in the file. Once the data was read in, I went ahead and used a for loop to iterate through the rows to convert them into a dictionary. I follow this with another for loop that took my dictionary and added it to a list with my column names, and created a new dataframe from that list. The final parts to this section were to split our names into two columns labeled first_name, and last_name. I utilized str.split() to do this with both, and then used drop to drop the name label. Then I reordered the columns and exported to the CSV labeled contacts.csv in our Resources folder. 

## ERD Diagram and SQL schema 

After all of our CSV files were completed, we utilized each one to create an ERD diagram and schema. Located within our project files are an image of the final ERD and the schema used to create it named crowdfunding_db_schema.sql. The other file in our project files is labeled crowdfunding_db.sql, and this is a SQL database created in PgAdmin 4 that created 4 tables each corresponding with our CSV files. We also imported each CSV file into their respective SQL table and finished off the code with Select * statements for each table to verify our data import was correctly completed. 

Two excel files located within Resources folder were provided in starter files for project 2 in module 13. Also starter code was provided to guide us. 