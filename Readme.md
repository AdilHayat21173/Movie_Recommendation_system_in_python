# Step-by-Step Guide to Movie Recommendation"

## Step 1: Download Dataset
1. Download the dataset from the following link: [MovieLens Dataset](https://grouplens.org/datasets/movielens/latest/)

## Step 2: Perform Exploratory Data Analysis (EDA)
1. Visualize the data based on the rating:
   - Count the number of ratings for each movie.
   - Calculate the mean rating for each movie.
2. Visualize the data based on the number of ratings each movie has received.
3. Create a few histograms to check the distribution of ratings and identify the most common rating (which is likely to be 3).

## Step 3: Recommend Similar Movies
1. Create a pivot table:
   - A pivot table is used to organize and analyze user ratings and preferences.
2. Apply the correlation method to find relationships between movies:
   - Calculate the correlation between movies, with values ranging from -1 to 1. The closer the value is to 1, the more correlated the movies are.
3. Sort the correlation values in descending order.
4. Create a DataFrame:
   - `corr_liarliar` is a DataFrame of movies similar to "Liar Liar," with their correlation scores.
5. Clean and organize the data:
   - Drop NaN values to remove any rows with missing data.
   - Add a column showing the number of ratings each movie received.
6. Filter and sort the data:
   - Keep only the movies with more than 100 ratings.
   - Sort the movies by correlation in descending order.
7. Display the top results:
   - Show the top similar movies based on the correlation scores.
