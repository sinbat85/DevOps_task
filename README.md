# DevOps_task
A pacrtical task to do for DevOps course listeners

We are going to build a community encyclopedia of birds. This website will :

Display the different entries submitted by the community, with the name and details of the bird they found.
Allow anyone to post a new entry about a bird that they saw.
This application will require three components :

The web server
The front-end (client side) app
The database

Prerequisites:
To run the server on your system:

Make sure you have dep installed
Run dep ensure to install dependencies
Run go build to create the binary (blog_example__go_web_db)
Run the binary : ./blog_example__go_web_db
To run tests:

Run dep ensure to install dependencies
Run go test ./...
Create the birds table before running the application :

create table birds (
id serial primary key,
bird varchar(256),
description varchar(1024)
);
Before running the application, edit the connString variable inside the main function to specify your postgres database connection