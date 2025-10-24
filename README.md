What It Does:

Uses the Requests library to send a GET request to the public Chuck Norris Jokes API
.

Receives a JSON response containing a randomly generated joke.

Parses the JSON data to extract and display the joke text.

Allows the user to continue requesting new jokes as many times as they wish.

Gracefully handles invalid inputs and exits the program when the user chooses to stop.

How It Works:
The program runs an infinite while loop that continues until the user enters 'N' or 'n'. Inside the loop, it checks the user's response:

If 'Y', it performs an API call using requests.get(), converts the response to JSON via .json(), and prints the joke stored under the "value" key.

If 'N', the loop breaks and the program displays a goodbye message.

Any invalid input triggers an error message and prompts the user again.
