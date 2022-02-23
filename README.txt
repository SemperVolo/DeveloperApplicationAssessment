# Aries Developer Application Assessment

Please see below steps for overview/instructions on setting up necessary data for running the developer application assessment:

---------------------------------------
---------------------------------------

1) General Info

 a) Download and Extract SankalpGodugu_DeveloperApplicationAssessment.zip (from this repository) to a location on your computer.
 
 b) Expand the Aries_DevAppAssessment folder, and you will see 3 folders within:
 
  > MyWebApi (API for interfacing between web app and database)
  > MyWebApp (Main web app)
  > SQL_Scripts (for creating relevant tables)
  > README (this file)

---------------------------------------

2) SQL Scripts to create database tables

 a) You will find the scripts for creating and populating the necessary tables in the /SQL_Scripts/ folder:
 
  /SQL_Scripts/Students.sql contains the logic for both creating the Students table and populating it with the provided sample data
  /SQL_Scripts/Contacts.sql contains the logic for both creating the Contacts table and populating it with the provided sample data

---------------------------------------

3) MyWebApi --> .NET Core Web API

 a) Navigate to /MyWebApp/ folder and open "MyWebApp.sln"
 
 b) Launch the application (non-debug mode)
  
  > if port# 44347 is occupied, feel free to change in launchSettings

---------------------------------------

4) MyWebApp --> .NET Core (MVC) Web App

 a) Navigate to /MyWebApi/ folder and open "MyWebApi.sln"

 b) Launch the application locally (non-debug mode) -- (ensure api project is already running from step #3)

  > if port# 44394 is occupied, feel free to change in launchSettings

---------------------------------------

5) Landing page (Students list display)

 a) MyWebApp should navigate to https://localhost:44394/
 
 b) You should land on a page displaying a table of students

  > The Contacts table should be empty until you click on a row in the students table, after which the contacts table will populate with the associated contact information for that selected student
