# Preparing the necessary libraries
## 1. ___import requests___ to make an API request
## 2. Store the website URL into a variable: ___base_url___ 
#### NOTE: Not necessary but it will make the code cleaner
## 3. Define a function whose goal is to pass the pokemon's name as the argument: ___def get_pokemon_name___
### a. Inside the function, a variable of URL is created. The URL is the official "link" to the pokemon data itself
### b. Calling the requests.get method will return a response object. We will then assign it to the variable ___response___
#### NOTE: TO see if the http response status code is optimal, ___print(response)___. (200-299 = Successful),  (400-499 = Client error), (500-599 = Server Error)
### c. Insert an if/else statement using the attribute __status_code__. If not 200, it will return an error.
### If response status code = 200, return the response in json format (key-value pairs): Assign ___response.json()___ to a variable: ___pokemon_data___

## 4. Outside the funcion: Create an if statement. If a pokemon's info (json file) is retreived successfully, the selected information will then be printed.
#### NOTE: By doing this, the data will be returned in a cleaner and more leggible way, since the dictionary itself is too big and display too many information.