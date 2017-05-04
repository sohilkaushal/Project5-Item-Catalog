This document contains following:
	1. Description of the project.
	2. Requirements for the project.
	3. How to execute the following project.


								**********  Project-Description  **********

This is project of making a item catalog website showing items of different category.
Registered users will have the ability to post, edit and delete their own items into the given database.


								**********  Requirements  **********

To run this project you should have the following things on your computer.
	1. Python
	2. Vagrant

								**********  Executing the project  **********

---------- For google authentication application

	1. Go to https://console.developers.google.com/project and login with Google.
	2. Create a new project and name it
	3. Select "API's and Auth -> Credentials -> Create a new OAuth client ID" from the project menu
	4. Select web application
	5. Now, on consent scree, type product name and save
	6. In Authorized javascript origins add: http://0.0.0.0:5000 http://localhost:5000
	7. Click create client ID
	8. Click download JSON and save to project folder by "client_secret.json"
	9. In login.html replace the line "data-clientid="xxxxxxxxxxx" with your client id from the web application.(The id's are included in clientid and secret.txt file).

---------- For setting the database and starting the server

	1. Copy the project folder any subfolders inside vagrant folder.
	2. Open terminal in the vagrant folder(For Windows :- by holding Shift key and then pressing the right mouse button and selecting open command prompt here).
	3. Type vagrant up.
	4. Now, type vagrant ssh
	5. Change the directory to the catalog folder.
	6. Type python database_setup.py
	7. Optional -- type python lotsofmenu.py
	8. Type python finalproject.py to start the server


That's it, now enjoy the webpage.

								************************ISSUES*************************

---------- Facebook authentication

1. The Facebook authentication using the link provided within the developer notes was tried.
2. But unfortunately it is not working for the moment.
3. The skeleton provided has been included inside the app for time being.

Credits ->
	1. Team Udacity.
	2. Stack Overflow Community
	3. Udacity Fourm

Extra Resources Consulted ->
	1. SQLalchemy Documentation
	2. Python Documentation
							 **********  Thank you  **********
