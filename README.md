# LEGO Set Explorer
This project involves building an interactive tool to aid quick exploration of all LEGO Sets, narrowing down the options based on certain criteria such as the set theme, age range, number of pieces and price. 
### Step 1: Data Collection
* The dataset was gotten from Maven Analytics Playground [Link](https://mavenanalytics.io/data-playground)
### Step 2: Data Cleaning
* Imported the dataset into Power BI.
* Removed unwanted columns.
* Reviewed column data types for accuracy, and filtered out records with no price, age, pieces or image URL values.
### Step3: Data Analysis
* Created conditional columns for Age Range (“Over 18”, “10 to 17”, “5 to 9”, “1 to 4”) and Price Range (>$500 = “$$$$$”, >$100 = “$$$$”, >$50 = “$$$”, >$25 = “$$”, otherwise “$”).
* Added measures to calculate the number of distinct sets (Total Sets) and theme groups (Total Groups), as well as the average age (Avg. Age), price (Avg. Price) and pieces (Avg. Pieces).
* Created a numeric range parameter (Max Price) ranging from 0-850 and incrementing by 5. A measure was also added to allow filtering of the table based on the maximum price selected.
### Step 4: Data Visualization
The visualization was done using Power BI. 
* The KPIs were created using the measures.
* Tooltips were enabled on the table to display the image of each LEGO set on hover.
* I made use of bookmarks and button actions to allow users to reset all filters on the page.
* Created a new report page with a decomposition tree visual to analyze Total Sets by category, theme group, theme and name.
* Added buttons to navigate between pages.

You can view the snapshot to my visualization below: 

![LEGO Set Explorer](https://github.com/user-attachments/assets/a6b598bf-215d-496b-833b-24d50dbc8dc4)

### Key Insights
1. The total number of LEGO Sets were 4,385; having average pieces of 411 and an average price of $45.
2. The most expensive LEGO Sets were "AT-AT" and "Millennium Falcon" which were both $849.99.
3. The cheapest LEGO Set was "Zombie" under the theme "Collectable Minifigures", year 2010, for children between 5-9, having average pieces 6, and average price of $1.99.
4. Theme-wise, "Star Wars" had the highest number of sets, amounting to 388, while "Stranger Things" had just a set. 

