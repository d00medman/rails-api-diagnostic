# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
Backends interact with data storage and provide data for the front end. They also allow for persistence and allow multi-user functionality
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
routes
```

Which layer in the MVC pattern communicates with the model?

```md
The controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Because they are entirely forward facing and entirely handled by the controller thus rendering them not really our problem
```

What does C.R.U.D stand for?

```md
Create Read Update Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
In the appropriate object controllers
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
Create -> POST -> create
Index -> GET -> read
Show -> GET -> read
Destroy -> DELETE -> destroy
update -> PATCH -> update
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
-The web server delivers the routes and appropriate resources to the controller
-Route sends a GET request to the server in the formate 'controller#method'
-controller sends the method to the model, which processes the request and sends it back to the controller.
-Controller sends it to the view, who renders the data appropriately.
-Data is packaged by the controller and sent back to the server.
-Server presents bata to the user
```

What is the command to generate a new rails-api app?

```bash
bin/rails generate scaffold post
bin/rails generate scaffold comment
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
bin/rake db:create
bin/rake db:migrate
bin/rake db:drop
bin/rake db:seed

```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold post name:string age:integer
```
