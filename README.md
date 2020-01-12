# JobPlacementDashboard

# Live Project

## Introduction
For the last two weeks of my time at The Tech Academy, I worked with my peers in a team developing a MVC Web Application. This was a great learning opportunity for fixing bugs, cleaning up code, and adding requested features. We were given the task of creating software designed to help hobbyists keep track of their collections of items, as well as interact with APIs and use DataScraping to get up to date information on things related to those collections and hobbies. This project was built using Python, Django, SQLite, and HTML/CSS. As this sprint was for only two weeks I was only able to work mostly on the [back end stories](#back-end-stories). Everyone on the team had the opportunity to work on front end and back end stories. Over the two week sprint I also had the opportunity to work on some other project management and team programming [skills](#other-skills-learned) which will be beneficial for any future projects.
  
Below are descriptions of the stories I worked on, along with code snippets and navigation links. I also have some full code files in this repo for the larger functionalities I implemented.

{% extends 'BasicApp/BasicApp_base.html' %}
{% load staticfiles %}
{% block templatecontent %}
<section>
    <div id="footyPic">
        <img src="{% static 'images/capturing_the_human_heart_travelApp_home.jpg' %}">
        <span class="footy_center"><strong>Welcome to the Travel App</strong><br />
            A collection of places to visit for a Hodophile! There's a database to manage
            countries visited and countries yet to be visited. It also includes an API which describes how dangerous a
            country is from a travellers perspective, and vacation ideas & popular destinations scraped from
            the website TripAdvisor. Take a look.</span>
        <br />
        <a class="footy_caption" href="https://unsplash.com/@dead____artist" target="_blank" rel="noopener noreferrer" title="Download free do whatever you want high-resolution photos"><span>Photo by Capturing the human heart.</span></a>
    </div>
</section>
{% endblock %}




















*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*

## Other Skills Learned
* Working with a group of developers to identify front and back end bugs to the improve usability of an application
* Improving project flow by communicating about who needs to check out which files for their current story
* Learning new efficiencies from other developers by observing their workflow and asking questions  
* Practice with team programming/pair programming when one developer runs into a bug they cannot solve
    * One of the developers on the team was having trouble with the JavaScript function being called to increment and decrement the likes on a page and myself and two others on the team sat with him and had him talk through what he had done so far. I asked questions about different ways to approach it until we found where it was broken and what needed to be fixed.
    * When a user requests a friendship there is supposed to be a pending notification displayed. One of the other developers was hitting a wall while working on this story when he discovered the functionality was working four different ways across the application. I sat with him and we talked through the process of each JavaScript function being called. We discovered there were multiple functions by the same name being loaded, so we simplified the code down to just one function. Clicking the button would now work from the nav drop-down but not on a specific page. I realized that the page was populating two different spans with the same ID and these were what was being targeted by the JavaScript function. So we needed to make that user-specific element identifier a class and target the class instead so that a change in either place would affect both.
  
*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*
