# TeSTing ReST

An introduction to what ReST (Representational State Transfer) is, how to *spy* on what a webpage is doing using developer tools and how to interact with a ReST API using Postman.

Visit [github.com/dcoomer/workshops](https://github.com/dcoomber/workshops) for the latest version of these workshops.

## Pre-requisites

1. Read through the introductory [slides](https://docs.google.com/presentation/d/1bQZlTnRyRi_cAuBmjn5QC97GYLN7lNqZ24Ee17G3TVk/edit?usp=sharing).
1. Download and install [Postman](https://www.postman.com/).  Its available for Windows, Linux and Mac.
1. Open Postman and create a new workspace (or use an existing one).
1. Import the Postman environments for the Restful Booker Platform
   1. The [Production](postman/production.postman_environment.json) environment references the Web UI version at [https://automationintesting.online](https://automationintesting.online)
   1. The [Heroku](postman/heroku.postman_environment.json) environment references the platform version at [https://restful-booker.herokuapp.com](https://restful-booker.herokuapp.com)
1. Import the [Postman collection](postman/restful-booker.postman_collection.json) for the Automation In Testing Restful Booker platform.

## Workshop

1. Explore the [Restul Booker](https://automationintesting.online) web application
1. Open your browser *Developer Tools* (usually by pressing *F12*)
   1. Create a few bookings with valid / invalid data
   1. Do you see anything interesting in the requests being sent by the web application using *Developer Tools*
1. Read through the [Restful Booker API documentation](https://restful-booker.herokuapp.com/apidoc/index.html) or as a [PDF version](restful-booker/restful-booker-platform-api-documentation.pdf) (extracted on 17 February 2020)
1. What can't you do through the Web UI?
1. Explore the Postman environment setup
   1. Environment level variables assist in exploring multiple environments
1. Explore Postman collection setup
   1. Collection level variables reduce maintenance by sharing values across various requests (e.g. for authorisation)
      1. Tests functionality can be used to programmatically set variable values
   1. Compare the request configuration and methods to the [Restful Booker API documentation](https://restful-booker.herokuapp.com/apidoc/index.html)
      1. Some requests don't work on both environments - can you find which ones?
1. Create and manipulate your own test data in the *Heroku* environment

## Further reading and information of interesting

1. [Restful Booker source](https://github.com/mwinteringham/restful-booker-platform)
1. [HTTP methods](https://restfulapi.net/http-methods/)
1. [HTTP Status Codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)
1. [URL encoding](https://www.w3schools.com/tags/ref_urlencode.ASP)
1. [API Testing from Entry Level to PhD](https://www.youtube.com/watch?v=KfQ95yLi58Y)
1. [the difference between ReST and CRUD](https://softwareengineering.stackexchange.com/questions/120716/difference-between-rest-and-crud)
1. [EvilTester ReST API Handout](https://www.compendiumdev.co.uk/downloads/workshops/htwtw/rest-apis-handout.pdf)
1. [API Security Breach - Facebook](https://www.helpnetsecurity.com/2020/02/17/api-security-facebook-breach/)
