# pandas-challenge
This is the submission for homework 4, the pandas homework.

Alright! Let's go over how I completed these!

Firstly, before reading through my code, I'd like to make it clear that I wanted to try multiple different methods of finding the answers as I was going through this.
I also believe that I got better at compiling code as I went through this from top to bottom. Pandas isn't my favorite to work with but I do believe I improved as I went through.

I start by importing my pandas and os dependencies, then use my os.path.join method to get the file path and import the .csv as a dataframe

From there I manipulate the dataframe to find the answers to each section, listed below.

# PLAYER COUNT

Here I create a new dataframe that is the number of unique screennames from the original dataframe and print that number out

# PURCHASING ANALYTICS

I find the average price, total number of purchases, and the number of unique items.
After finding each I format them then put them into a dataframe

# GENDER DEMOGRAPHICS

For this I find the attributes for each gender group, the total count and percentage of players, then put them in their own dataframe
Then I make a final dataframe as a copy of the first gender then append the others onto it to get the final result

# PURCHASING ANALYSIS (GENDER)

I create a dataframe for each of the attributes I need, the total count, average price, total purchase value, and average total per person.

Then I merged each of these dataframes together to get the final result

# AGE DEMOGRAPHICS

I create bins for each of the age groups and name them before pulling them into a dataframe using the .cut fuinction.

Then I drop the duplicates in the screen name column to avoid data bias

Final I do my count and percentage calculations and sort by the ages

# PURCHASING ANALYSIS (AGE)

I create a groupby item and convert that into separate dataframes for each of my attributes

Then I merge the attributes into a single dataframe and rename the columns

# TOP SPENDERS

I create a groupby item and convtert that into separate dataframes for each of my attributes

Then I merge them into a single dataframe and rename the columns

# MOST POPULAR ITEMS

I create a new dataframe that is filtered to just the item ID, Item Name, and Price.

Then I group them by Item ID and Item name

Then I put my attributes in new dataframes, merge them together, and rename before sorting.

# MOST PROFITABLE ITEMS

I use 2nd half of the code from above but sort by Total Purchase Value rather than Purchase count.