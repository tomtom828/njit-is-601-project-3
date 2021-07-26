# IS 601 - Project 3


## Project Description
This project's goal was to use a REST API and use Postman to test the GET, POST, PUT, and DELETE request methods.

The data was taken from [this](https://people.sc.fsu.edu/~jburkardt/data/csv/csv.html) csv source and converted to SQL statements using [this](https://sqlizer.io/#/) online tool.


## API Endpoint Testing using Postman
As the project was built, each API endpoint was manually tested using Postman. The screenshots below show the results.

### Get All Players
API Endpoint of `localhost:5000/api/vi/players` with a `GET` request.
![api_all_players](screenshots/postman-get-all-players.png)

### View a Single Player By Id
API Endpoint of `localhost:5000/api/vi/player/:id` with a `GET` request for a given player `:id`.
![api_get_player](screenshots/postman-get-player.png)


### Add a New Player
API Endpoint of `localhost:5000/api/vi/player` with a `POST` request containing the JSON body playload below.
![api_post_new_player](screenshots/postman-post-new-player.png)

Note that we can query for all players again and see that the new player was added below.
Also note that the player id is 101 since the database will automatically increment the primary key.
![api_get_new_player](screenshots/postman-get-new-player.png)


### Update an existing Player
API Endpoint of `localhost:5000/api/vi/player` with a `PUT` request containing the JSON body playload below.
![api_put_update_player](screenshots/postman-put-update-player.png)

Note that we can query for the player by id again and see that the existing player indeed updated.
![api_get_update_player](screenshots/postman-get-update-player.png)

