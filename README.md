# F18507FinalProj
This final project works with the Harvard Art Museum's API, resources for which can be found here: https://github.com/harvardartmuseums/api-docs
This project also uses the Google Books API, resources for which can be found here: https://developers.google.com/books/docs/v1/getting_started

You will need an API key for the Harvard API, but not for the Google Books one. The Harvard API Key can be obtained by clicking the "send a request"link found in the README doc for the API, linked above.

You will also need to have the Plotly package installed on your computer, and have a Plotly account and API key in order to run this program. Help for getting started with Plotly can be found here: https://plot.ly/python/getting-started/

You will need to save your Harvard API key, Plotly username, and Plotly API key into a file named secrets.py and hold each piece of information in variables named HARVARD_API_KEY, PLOTLY_USERNAME, and PLOTLY_API_KEY respectively. This file is imported into the main files of the program as a module.

The code for this program is structured into two main files (with a third tests file). The first main file is data_gather.py This file can to be run in order to gather the initial data from both APIs and then build it into a database (using sqlite3). Please note that some of the api calls can take a while to run (i.e. a few hours) and building the database after this point can also take some time. For that reason a completed version of the database is also included in this repository called art.db so that all of the data can be accessed this way instead of through having to call the APIs.

The second file runs the main functionality of this program. It is called final_proj.py This file includes five functions that create the main visualizations for the project, they are titled make_culture_bar, artists_from_culture, gender_bar, get_objects, and get_books. There is then also a function to prompt the user for what kind of information they would like to explore, one of the first five functions are then called based on their response. The user can continue to explore any of the five options until they enter 'quit' to exit the program. There is also the option in the interactive prompt for the user to enter 'help' so they can see a list of available commands and what each one does.

In order to run the program successfully, make sure that art.db, secrets.py and final_proj.py files are in the same directory. Run the final_proj.py file and make sure that the function interactive_prompt() is called. This will start the interactive features of the program. When running the program for the first time, enter 'help' as the first command in order to see instructions for the other available commands.
