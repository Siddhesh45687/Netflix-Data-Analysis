

# Netflix Data Analysis 

This project focuses on exploring and understanding a Netflix movies dataset.
The goal is to clean the data, organize it properly, and create simple charts to learn more about movie trends.

## 1. Importing the Required Libraries

We start the project by importing important Python libraries like:

* **pandas** – for working with data
* **numpy** – for basic operations
* **seaborn** and **matplotlib** – for graphs and visualization

These tools help us read the dataset and create charts.

## 2. Loading the Dataset

We load the `netflix.csv` file using pandas.
Then, we check the first few rows to understand the structure of the data.

## 3. Checking Data Information

We use:

* `df.info()` → to see column names and data types
* `df.isnull().sum()` → to find missing values
* A heatmap → to visually check where data is missing

This helps us understand what cleaning is needed.

## 4. Cleaning the Data

We perform several cleaning steps:

### ✔ Convert text columns into numbers where needed

Columns like:

* *Vote_Count*
* *Popularity*
* *Vote_Average*

are converted from text to numeric form so that we can analyze them.

### ✔ Removing missing values

We drop rows with missing data using `df.dropna()`.

### ✔ Removing unnecessary columns

Columns like:

* *Overview*
* *Original_Language*
* *Poster_Url*

are removed because they are not needed for the analysis.

##  5. Converting the Release Date

The *Release_Date* column is changed from text to a year format.
This helps us to study which year had the most movies released.

##  6. Categorizing the Vote Average

We convert the *Vote_Average* column into 4 simple groups:

* **not_popular**
* **below_avg**
* **average**
* **popular**

This makes it easier to compare movies based on rating.

##  7. Splitting the Genre Column

Movies often have more than one genre.
So we split the *Genre* column and create a separate row for each genre.

This helps in finding the **most common movie genres**.

## 8. Changing Genre to Category Type

We convert the Genre column into a "category" data type.
This improves performance and helps in analysis.

## 9. Data Visualization

We create different charts to understand the data:

### ✔ Most common genres

A bar chart showing which genres appear most in Netflix movies.

### ✔ Vote Average distribution

Shows how many movies are:

* popular
* average
* below average
* not popular

### ✔ Most popular movie

Finds the movie with the highest popularity score.

### ✔ Least popular movie

Finds the movie with the lowest popularity score.

### ✔ Release year trend

Shows which year had the highest number of movies.

### Top Genre Movie

This show Top 5 genre movie in Netflix



