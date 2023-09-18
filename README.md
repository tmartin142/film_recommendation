# A Recommendation Engine for Classic & International Films
For this project I have created a function where a user can input the name of a film and receive recommendations for either classic or international films.

### Objective
My main goal for this project is to assist people who enjoy watching films to broaden their horizons and experience new areas of film.

In order to achieve this goal, I aimed to create a film recommendation tool where the user inputs a modern film that they enjoy, and the tool provides recommendations of either classic films or foreign films that the user might also like. 

This way it can provide a personalised starting point for people to branch out from modern English-language films.

### Data Used
This project uses the MovieLens film data which can be downloaded here:

https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset

The following files are used:

- `ratings.csv` - a dataset of 26 million user ratings
- `movies_metadata.csv` - a dataset providing details for each film
- `links.csv` - a dataset linking id numbers between each dataset
- `keywords.csv` - a dataset of keywords associated with each film

### How to Use
The file `film_recommendation_project.ipynb` contains the full breakdown of the project with data exploration, visualisations, and different iterations of the final recommendation engine.

The file `recommendation_function.ipynb` contains only the code required for the final function to be usable.

The final recommendation engine is a simple function. The input is a film title as a string. It is not case sensitive and ignores any punctuation.

If there is more than one film with that title, the function will prompt you to give a release year, and will then use the film released closest to the year provided.

By default, the function will return recommendations for classic films. You can request recommendations for international films by adding the argument 'international = True'.
