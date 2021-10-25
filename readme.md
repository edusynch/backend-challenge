# EduSynch Backend Challenge

Fork this repository
Create a new rails project
Submit a pull request

## Todo API endpoints

## Documentation

### Get All Todos
----
  Returns json data with all todos.
  
  | URL | Method | Params | Data Params | Success response | Error response|
  |--|--|--|--|--|--|
  |`/todos`|GET|None|None|Status 200||


**Get Todo**
----
  Returns json data about a single todo.
  
  | URL | Method | Params | Data Params | Success response | Error response|
  |--|--|--|--|--|--|
  |`/todos/:id`|GET|`id=[ObjectId]`|None|Status 200|Status 404|

**Create Todo**
----
  Returns json data about the created todo.
  
  | URL | Method | Params | Data Params | Success response | Error response|
  |--|--|--|--|--|--|
  |`/todos`|POST|None|`title=[String]`|Status 200|Status 400 |

**Update Todo**
----
  Returns json data about the updated todo.
  
  | URL | Method | Params | Data Params | Success response | Error response|
  |--|--|--|--|--|--|
  |`/todos/:id`|PUT|`id=[ObjectId]`|`title=[String]`|Status 200|Status 400 |


**Delete Todo**
----
  Returns json data about the deleted todo.
  
  | URL | Method | Params | Data Params | Success response | Error response|
  |--|--|--|--|--|--|
  |`/todos/:id`|DELETE|`id=[ObjectId]`|none|Status 200|Status 400 |


- [ ] Deploy your app to [Heroku](https://heroku.com). The link to the deployed API is your submission deliverable

### Important Notes

- You need make the API connection with some database MySQL / PostgreSQL, if other put into the pull request comment.
- Alternatively you can use an in-memory array to persist users and act as a database, and build database helpers that interact with the users array.

### Stretch Yourself

- Make the API authenticatable, create users (you can use the seeds for that), and use [JWT](https://jwt.io) to authenticate it.
- Research how to avoid storing plain passwords as is in your array database.
- Research how to grant access to `/todos` only those clients that are registered and logged in.
- Create unit tests using RSpec, Cucumber or any other testing framework that you are confortable with.
- Create docker files for deployment / test (Dockerfile and docker-compose.yml)