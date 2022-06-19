<-- full stack mern app using graphql and apollo client -->

### Backend (server)
## initialize graphql schema with our sample data. 

## run the queries for project and the clients.
## initialize a mongodb database and make the schema.


``` 
───server
│   index.js           # main file
│   sampleData.js      # our sample data 
│   
├───config
│       db.js          # mongodb database 
│       
├───models             # mongoose models
│       Client.js     
│       Project.js
│
└───schema
        schema.js      # graphql schema

```



### Frontend (client side code)
## initialized client with *react and apollo/client*


```
───client
│   App.css
│   App.js                    # main js 
│   index.css                 # our css with fonts we are using
│   index.js
│   
├───components
│   │   AddClientModal.jsx    # client modal to add the client
│   │   ClientRow.jsx
│   │   Clients.jsx
│   │   Header.jsx
│   │   ProjectCard.jsx
│   │   Projects.jsx
│   │   Spinner.jsx
│   │
│   └───assets
│           logo.png          # graphQL logo
│
├───mutations
│       clientMutations.js    # client mutations
│
├───pages
│       Home.jsx
│       NotFound.jsx
│       Project.jsx
│
└───queries
        clientQueries.js      # client queries
        projectQueries.js     # project queries
```


##  client queries
   **created client queries to get the clients**
- this will create a query to get all the clients.
- and will return the id name email and phone of the client.

##  project queries
   **created project queries to get the projects**
- this will create a query to get all the projects.
- as well as will return us the projects information like id name and status of the project.
## client mutations
   **created mutation to get and delete the client**
- this will create a mutation to add client and delete client with gql and will return the rest information(id,name,email,phone). 

## AddClientModal and DeleteClient will update the query with cache and fetch the query(just so we won't have to reload after every add and remove). and as well as app.js will fetch the query and merge it to solve existing and incoming issue. 