# Building an API With Spring

So far we've been looking at tools which will help us store and manipulate data. We can also design APIs to let other applications access that data. If the API is designed in a certain way (eg. following a RESTful pattern) then any developers using it in future will have some idea of what to expect.

As BNTA expands there are going to be many more consultants and clients to keep track of, so having some sort of database with a consistent way of interacting with it would be really useful. That's where you come in...

## Task

Your task is to build a simple database to hold details of BNTA's consultants and clients along with an API to interact with it. Your database should include tables for:

- **consultants**, which will hold details of:
	- name
	- location
	- are they able to relocate?
	- current client

- **clients**
	- name
	- sector (eg. finance, law)
	- location
	- required number of consultants

Your API will need routes to:

- add a client
- add a consultant
- view all clients
- view all consulatants
- view individual clients
- view individual consultants
- update a consultant with new location and/or cient details
- view all consultants working at a given client
- view the client a given consultant is working for

## Extensions

- Some consultants may need to go on additional specialist training courses, eg. for mobile development. Add a **courses** table to store details of them.
- We'll need a record of which consultants have been on which courses, and also of which clients require their team to have taken which courses. Add tables to track those details.
- Add a route to the API to view all consultants who could work for a given client, ie. those who:
	-  have done the required courses
	-  are in the right place
	-  are willing to relocate if not