# JobPlacementDashboard

# Live Project

## Introduction

For the last two weeks of my time at The Tech Academy, I worked with my peers in a team developing a MVC Web Application. This was a great learning opportunity for fixing bugs, cleaning up code, and adding requested features. We were given the task of creating software designed to help hobbyists keep track of their collections of items, as well as interact with APIs and use Data Scraping to get up to date information on things related to those collections and hobbies. This project was built using Python, Django, SQLite, and HTML/CSS. this sprint was for only two weeks I was only able to work on some front and back end stories. Everyone on the team had the opportunity to work on front end and back end stories. Over the two week sprint I also had the opportunity to work on some other project management and team programming [skills](#other-skills-learned) which will be beneficial for any future projects.
  
Below are descriptions of the stories I worked on, along with code snippets and navigation links. I also have some full code files in this repo for the larger functionalities I implemented.


## Travel App Homepage
The following code is for the homepage I built for my Travel App. 

![TravelApp_homepage_Code](https://user-images.githubusercontent.com/41709286/72227291-c0753880-3568-11ea-9f15-c83d6b542af8.PNG)

![travelApp_homepage](https://user-images.githubusercontent.com/41709286/72227658-66c33d00-356d-11ea-89c3-e459306b00e9.PNG)

## Travel App Model 
With Django, you don’t have to use SQL (unless you want to), instead, you use a Django Model to access the database. So, for this project we used the Django Model to access the database. The models.py is mapped to the database and when you create a model, Django executes SQL to create a corresponding table in the database. The Django Model contains the essential fields and behaviors of the data we were storing and here in this app it kept track of details related to a trip. 


![TravelApp_modelSchema](https://user-images.githubusercontent.com/41709286/72228090-9116f980-3571-11ea-9900-d1d9bc69901b.PNG)


## Travel App Index Page (Add Function) 

The Index page for the Travel App displayed the information from the database.The index page, was linked from the home page and it displayed the list of trips in the database, with all of the fields for a specific trip displayed with labels/headers. There was a add function to add the trips to the database and got all the items from the database and finally redirected the trips to the template. 

![TravelApp_AddFunction](https://user-images.githubusercontent.com/41709286/72289586-6f714d00-3619-11ea-987e-2c4b48f08843.PNG)


![TravelApp_IndexPage](https://user-images.githubusercontent.com/41709286/72289799-da228880-3619-11ea-8619-b88e47ead054.PNG)


## Travel App Details Page (Detail Function)

The details page displayed the details of any single trip from within the database, as selected by the user. The details page was linked to the index page with a button for each trip. The function created in views.py file locates the single desired instance from the database and sends it to the template. When the details button is clicked in the index page for any of the trip it takes the user to the details page displaying all the details of the specific trip chosen. 

![TravelApp_detailsPage](https://user-images.githubusercontent.com/41709286/72290146-92e8c780-361a-11ea-8a35-b6dbb9f9e94f.PNG)


![TravelApp_details](https://user-images.githubusercontent.com/41709286/72290614-a2b4db80-361b-11ea-9002-49d928c262aa.PNG)



*Jump to: [Other Skills](#other-skills-learned), [Page Top](#live-project)*

## Other Skills Learned
* Improving project flow by communicating about who needs to check out which files for their current story 
* Practice with team programming/pair programming when one developer runs into a bug they cannot solve
    * One major issue that I stumbled upon was my index page did not render intially when I was running the server for my app. My initial thought was it could be that it was an url issue. However, after several tries that wasn't the case. This lead me to push my code to the remote repository and debug with one of the project leaders. The page did render for the project leader and it was working just fine for them. The issue lied on my end  so after couple hours of debugging with the project leader we tried getting rid of all the migration files for the project and deleting the database from my side. After, deleting those files I ran the following commands: python manage.py makemigrations & python manage.py migrate. Then, when I ran the server now the page finally rendered on my side. So, we figured the issue lied in the database on my side. 
   
  
*Jump to: [Other Skills](#other-skills-learned), [Page Top](#live-project)*
