# API Rest with Gorilla Mux

>This GO code is a simple implementation of an API REST using the Gorilla/Mux framework, which is a popular package for web applications with GO. API allows you to create, recover and delete information about people stored in memory.

## Data structure

* Person: It represents a person containing an id, name, surname and an optional address.
* Address: It represents an address containing city and state.

## List of People

* people: A slice variable that stores a list ofPerson.

## Functions of API
* GetPeople: Returns all people stored inslice people.
* GetPerson: Search and returns a specific person by ID.
* CreatePerson: Creates a new person and adds to Slice People.The ID is obtained from the URL.
* Deleteperson: Delete a Slice People person based on the supplied ID.
## Routes
* /Contact: Using the GET method, you call Getpeople to get all contacts.
* /contact /{id}: depending on the http method:
* GET: Returns a specific contact via Getperson.
* Post: Creates a new contact via Createperson.
* Delete: Delete a contact via Deleteperson.
## Server Execution
* The server is configured to run at the local address on port 8000, using the router configured for the routes mentioned.
## Initial behavior
* Program startup, two entrances to Slice People for test purposes are pre-filled.
## Use
To test this API, you can use tools like Postman or Curl.For example, to get all contacts, you can send a GET request to localhost: 8000/contact.To add, access a specific contact or delete, you use the localhost URL: 8000/contact/{id} with the appropriate method.

This code is a basic example and serves well to understand how rest apis are created and manipulated in GO using gorilla/mux.

Clone the project locally:

```sh
$ git clone git@github.com:RodrigoPinheiro67/apiRestMux.git
```


