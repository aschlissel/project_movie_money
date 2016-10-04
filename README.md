# Project Movie Money  
  
This was my first independent data science project. I wanted to practice my web scraping skills and learn about linear regression using Python and sci-kit learn.  
  
In this project, I envisioned my client to be someone deciding whether to invest in a movie in the late stage of production. So in my case, the genre, budget, and MPAA rating would have already been established.  
  
To do this, I looked at historical data about the most successful movies to see which traits they had in common. I considered the most statistically significant indicators, which had a p value of 0.1:  
- Budget was by far the most correlated to the worldwide gross of a movie.  
- The genres most indicative of a movie's success were: Action/Comedy, Action/Fantasy, Concert, Fantasy, Foreign, Period/Horror, Sci-Fi/Adventure, Sci-Fi/Fantasy, Sci-Fi/Horror  
- Interestingly enough, MPAA rating was not significant. I thought it may be significant because rated R movies exclude two significant demographics who go to movies, namely, families and kids under 17.  
  
On the technical side, I scraped my data from boxofficemojo.com using BeautifulSoup. I scraped the top 500 world wide grossing movies with their runtime, domestic total gross, genre, production budget, and worldwide gross. I used Lasso Regression because it performed both variable selection (since I didn't know which variables would be the most important) and regularization to increase the model's accuracy. Lasso is great for feature selection because it penalizes the absolute size of the regression coefficients.
