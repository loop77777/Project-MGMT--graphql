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

## initialized client with _react and apollo/client_

```
───client
│   App.css
│   App.js                    # main js
│   index.css                 # our css with fonts we are using
│   index.js
│
├───components
│   │   AddClientModal.jsx    # client modal to add the client
│   │   AddProjectModal.jsx   # project modal to add projects
│   │   ClientInfo.jsx        # for the view page
│   │   ClientRow.jsx
│   │   Clients.jsx
│   │   DeleteProjectButton.jsx
│   │   EditProjectForm.jsx   # to edit the project information
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
│       projectMutations.js   # our project mutations
│
├───pages
│       Home.jsx              # homepage
│       NotFound.jsx          # 404
│       Project.jsx           # project component
│
└───queries
        clientQueries.js      # client queries
        projectQueries.js     # project queries
```

## client queries

**created client queries to get the clients**

- this will create a query to get all the clients.
- and will return the id name email and phone of the client.

## project queries

**created project queries to get the projects**

- this will create a query to get all the projects.
- as well as will return us the projects information like id name and status of the project.

## client mutations

**created mutation to get and delete the client**

- this will create a mutation to add client and delete client with gql and with return the rest information(id,name,email,phone).

## project mutations

**created mutations to add, update and delete the projects**

- this will create, update and delete the projects.
- the projects we make will associate with one of the clients.

## AddClientModal and DeleteClient will update the query with cache and fetch the query(just so we won't have to reload after every add and remove). and as well as app.js will fetch the query and merge it to solve existing and incoming issue.

## Business logic

### Add Client

`this will add the clients with name, email and phone.`

### Main Page

`here if we delete the client it will delete all of its projects too`
**on the page we can view the projects, update the information as we needed and can delete the project.**

### Add Project

`it will make a project with project name , project status(not-started, in-progress or completed) and the client`
