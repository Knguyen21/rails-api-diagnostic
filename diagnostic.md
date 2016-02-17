# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
The puropse of a backend is to save data. It allows data to persist when browser is closed.
In addition, it allows two users to interact with each other in the app
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
model fetches data in the database
```

Which layer in the MVC pattern communicates with the model?

```bash
controller(lazy- most often skinny- manager) communicatese with the model
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
We do not need views . We are using our own view layer. My Question(when there it is a single page app, is the view neccessary?).
```

What does C.R.U.D stand for?

```bash
Create read update destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
The controller
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
-browser fires a request to the webserver,
-the webserve goes to the router.
-route indicate to the server which controllers should be triggered (and how) by which kinds of requests
- then the controller ask model to do a 'GET' request for 'person/1'
-Model talks to database and make the 'GET' request and retrieves the data from the database
- Model then gives the data to the controller.
-  Controller than gives it to view to display.
```

What is the command to generate a new rails-api app?

```bash
gem install rails-api
the next step to create an app is to type this in the terminal: rails-api new blog_app --skip-javascript --skip-sprockets --skip-turbolinks --skip-test-unit --database=postgresql

```

What is the command to start an instance of a rails server?

```bash
rails s
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
- rake db:create
- rake db:migrate
- rake db:drop
```

What is the command to scaffold a pet with a name and an age?

```bash
rails-api g scaffold pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
- makes api safer to use
- it helps keep your code DRY
- makes api easier to use
- you can combine different models, through serializers, into a same JSON response
- http://www.thecodeknight.com/post_categories/web_development/posts/rails_json_apis (resource)
```
