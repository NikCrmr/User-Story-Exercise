# User Story 1

## List of Current Movies

## Value Proposition

As a User
I want to see a list of movies,
so thatI have an overview of all movies

## Description

- see a list of movies in a grid. 2 movies in a row. a poster of a movie or a recognizable displaying each movie.
- in the right-top corner is a number from 0-10, which give the ratings of the movie.
  -Below the movie image the title of movie is displayed.
- if an error occurs in the data laoding process a error page occurs.
  "Sorry, we couldn't retrieve the latest movie data
  at the moment. Please try again later."

<img src="Bildschirmfoto 2024-02-16 um 10.06.22.png" height="400px">

## Acceptance Criteria

- the user can scroll vertically to display the list of movies
- the user can click on a movie to display details about it
- the user can see the rating of the movie
- the user gets an error if content isnt loading
- the user sees a centered title at the top of the page with the name of the app: "movie app"

## Tasks

Technical explanations: from developers for developers

- create a list of movies or use an existing movies list database. The database has to include an id, the movie name, desription, an movie image, a title and a rating.
- create a component where you display the list of movies.
- link the movies list to the app component(in react) homepage component in nextjs.
  -create an error handling and add following error message:
  "Sorry, we couldn't retrieve the latest movie data
  at the moment. Please try again later."

---

# User Story 2

## Movie detail page

## Value Proposition

As a User
I want to click on a movie and see more information
so more information about the movie

## Description

- Each movie tile on the homepage is clickable and leads you on the detail page with more information about the movie.
- on the detail page the is a title of the movie, a release date, an image and a description.
- on the top of the app screen is the app-title displayed. like on the homepage. left beside the title there is a back arrow, which leads you back to the movie list.

<img height=400px alt="Detailpage Wireframe" src="Bildschirmfoto 2024-02-16 um 10.21.56.png">

## Acceptance Criteria

- the user can click on a movie image and is lead to a detail page with detailed informatzion about the movie.
- on the detail page there he sees following information.
  Title, release date, an image of the movie and a description.

## Tasks

Technical explanations: from developers for developers

- create a MovieDetailPage Component.
- add an h1 for the title with styled components.
- add a release date and an movie image.
  -add the release date to the database.
- import the data dynamically.
  -add an description.
  -add a back arrow so that the user can go back to the movie list

---

# User Story 3

## Watchlist

## Value Proposition

As a User
I want to add movies to a watch list
so i can know which movies i want to watch.

## Description

On the Homepage:

- On the homepage you have now added a footer navigation-bar. There are two options.

1. Home (for the Homepage)
2. Watchlist (for the Watchlist)

On the Movie Detail Page

- there you have centered below the movie description a squared button with the text "Add to watchlist"

On the Watchlist

-a title with "Watchlist"

- when the watchlist is empty following text:
  "Your watchlist is currently empty. Start adding
  movies you want to watch by clicking
  'Add to Watchlist' on the movie details page.
  Your selected movies will appear here."
- When movies are added to the watchlist, the list of watch list movies are displayed.

<img height=400px alt="Watchlist Wireframe" src="Bildschirmfoto 2024-02-16 um 10.36.39.png">

## Acceptance Criteria

On the Homepage:

- The user has a menu a the footer of the screen and can select between "Home" and "Watchlist".
  On the Detail Page:
- The User can click on a button "Add to watchlist" and the movie on this page can be added to the watchlist.
  On the Watchlist:
- The user sees a list of movies he want to watch.

## Tasks

Technical explanations: from developers for developers

- create a navigation component and add it to the home page and later to the watchlist.
- add a button "Add to Watchlist" to the Movie Detail Page below the description, centered.
  -Create a "Watchlist" Component and A a list of movies. Similiar like the homepage but only one movie in one row. Also add the Navigation bar on this side.
