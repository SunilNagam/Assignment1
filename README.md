# Assignment1
Voting Application
Project Description

This project is a simple voting application where users can vote for candidates using web URLs. The application keeps track of how many votes each candidate receives. Users can also view the current voting results. Version 2 adds an option to reset all votes.

Installation and Setup
1. Clone the repository
git clone https://github.com/SunilNagam/Assignment1.git
cd Assignment1

 Start the application
python app.py


The application will run on:

http://localhost:5000

API Endpoint Reference

/	            GET	Displays the application welcome message	Welcome to the App
/health	        GET	Checks whether the application is running	App is running
/vote/<name>	GET	Records one vote for the specified candidate	{"message":"Vote recorded for <name>","votes":1}(if called  with the same name vote count increases)
/results	    GET	Displays the current vote count for all candidates	{"candidate1":2,"candidate2":1}
/reset	        GET	Clears all stored votes	{"message":"All votes have been reset"}

Example Usage

To vote for candidate1:

http://localhost:5000/vote/candidate1


To vote for candidate2:

http://localhost:5000/vote/candidate2


To see the results:

http://localhost:5000/results


To reset all votes:

http://localhost:5000/reset

