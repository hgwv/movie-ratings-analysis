# Movie Ratings Analysis

## Goal
The goal of this project is to explore which movie attributes are associated with higher IMDb ratings and to evaluate whether commonly assumed factors—such as runtime or release decade—show measurable relationships. This analysis uses basic Python data analysis and visualization techniques.

---

## Dataset
- **Source:** Kaggle (uploaded by Harshit Shankhdhar)  
- **Number of movies:** 1000  
- **Columns used:**
  - `Series_Title`
  - `Released_Year`
  - `Runtime`
  - `Genre`
  - `IMDB_Rating`

---

## Questions
- What is the average IMDb rating of movies in this dataset, and how are ratings distributed?
- How have IMDb ratings changed over time, and are there noticeable trends across decades?
- Is there a measurable relationship between movie runtime and IMDb rating, or is the relationship weak?

---

## Method
- Selected relevant columns from the original dataset
- Converted text-based columns into numeric values where necessary
- Handled missing and inconsistent values
- Grouped movies by release decade for temporal analysis
- Created visualizations using `matplotlib` to explore distributions and relationships

---

## Results
- The average IMDb rating in the dataset is approximately **7.95**, with most ratings clustering between **7.5 and 8.5**.
- IMDb ratings remain fairly consistent across decades (generally between **7.9 and 8.1**), suggesting that highly rated films appear in all eras rather than being concentrated in a specific time period.
- The scatter plot of runtime versus IMDb rating shows **no strong linear relationship**, indicating that longer movies are not consistently rated higher than shorter ones.

---

## Visualizations

### Distribution of IMDb Ratings
![Distribution of IMDb Ratings](/images/ratings_distribution.png)
This histogram shows that most movies in the dataset fall within a narrow rating range, with relatively few extreme values.

---

### Average IMDb Rating by Decade
![Average IMDb Rating by Decade](/images/avg_ratings_by_decade.png)
This bar chart demonstrates that average IMDb ratings have remained relatively stable across decades.

---

### Runtime vs IMDb Rating
![Runtime vs IMDb Rating](/images/runtime_vs_rating.png)
This scatter plot illustrates the weak relationship between movie runtime and IMDb rating.

---

## Limitations
- The dataset includes only 1000 movies and may not represent all IMDb films.
- Other potentially important factors (such as budget, director, cast, or number of votes) were not analyzed.
- This analysis identifies correlations only; correlation does not imply causation.

---

## Next Steps
- Analyze IMDb ratings by genre to identify potential differences across categories.
- Incorporate additional features such as number of votes or director to improve the analysis.
- Use larger or more diverse datasets for stronger conclusions.
- Apply basic statistical measures (e.g., correlation coefficients) to quantify observed relationships.
