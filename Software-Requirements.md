#  Software Requirements 

## Product vision
- Tourism site that renders a map for a city based on user input. We will render a map that shows the city on one page and a form at the bottom of that page where the user can input trip data and save it to their profile.On the profile page, we will display all trip itinerary data for the given user. The user will have the ability to update and delete existing trip data.



## Pain point this project solves
- Traveling can be hard and our site is just trying make that a little easier. On our website you can search a city and food type to gather related restaurants in that area. 


## The why behind our product
- Our website provides a streamlined access to nearby restaurants making your trip that much easier. 


### Scope (In/Out)
- IN - What will your product do
  - website will have landing page that requires you to login with Auth0
  - After logging in user can input a city and food type of their choice which then displays top restaurants related to their search.
  - a user can add restaurants they want to try/visit.
  - the user can edit notes on the added restaurants on their profile page.
  - provide an about me page that shows all employees and developers of site.



- OUT - What will your product not do.
  - website will not turn into an IOS or android app
  - does not display reviews on the restaurants 
  - it will not render a map 
  - you will not be able to change the restaurant data.



## MVP functionality
- Initial page(home page with auth0 login)
- On login it displays a page with a form that allows the user to input a city
- Once a city is entered the page renders a map and a  form that allows you to add/create  trip data
- Button to redirect to profile(page) that has saved trip data
- User then can read update and delete trip data from profile  page
About us page.



## Stretch goals
- filter by rating
- better css 
- map 
- cache the same api calls 

## Functional Requirements
- user can search city and food type
- user can make add restaurants to their profile
- user can make notes on each restaurant 
- user can delete a restaurant from their profile. 

## Data Flow
1. user arrives at home page, shown an auth0 login
2. user then is shown after logging in with aut0 a form that accepts city and food type as input.
3. user then is shown a list of restaurants from input. 
4. user can click on a restaurant and add it to their profile 
5. user then navigates to their profile and is shown added restaurants.
6. user can make notes on their added restaurants. 
7. user then can choose to delete their restaurant.

## Non-Functional Requirements (301 & 401 only)
  
  ### Usability
      
  - If there are too many api calls the site will no longer add
       and other restaurants. also if the api limit is hit then the 
       data will look very cluttered on the profile page; we are not 
       sorting the data. 

  ### Security
  - If auth0 is down the user won't able to login to our site and
       access the data correctly. Make sure our .env file is not on 
       our github. People only have access to the sample.env and not 
       our api links, mongoDB links.
