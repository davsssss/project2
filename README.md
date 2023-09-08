# project2

Crowdfunding Extract, Transform, Load

David: I started by creating the 'category' and 'subcategory' dataframes. To complete this I started by splitting the 'category & subcategory' column from the crowdfunding.xlsx into individual lists and getting the unique values. I then created unique ID's for each given category and subcategory using list comprehension. I then created a category dataframe using the category_id and category list (same for subcategory). Then I created the campaign dataframe by using the required columns from the crowdfunding.xlsx. After getting the required columns changed the 'goal' and 'pledged' datatypes to float along with changing the names and datatypes of the 'launched_at' and 'deadline' columns. All created dataframes were saved to their own .csv. All instructions came from project 2 in module 13.
