# Battlesnake Python Starter Project

An official Battlesnake template written in Python. Get started at [play.battlesnake.com](https://play.battlesnake.com).

![Battlesnake Logo](https://media.battlesnake.com/social/StarterSnakeGitHubRepos_Python.png)

This project is a great starting point for anyone wanting to program their first Battlesnake in Python. It can be run locally or easily deployed to a cloud provider of your choosing. See the [Battlesnake API Docs](https://docs.battlesnake.com/api) for more detail. 

[![Run on Replit](https://repl.it/badge/github/BattlesnakeOfficial/starter-snake-python)](https://replit.com/@Battlesnake/starter-snake-python)

## Technologies Used

This project uses [Python 3](https://www.python.org/) and [Flask](https://flask.palletsprojects.com/). It also comes with an optional [Dockerfile](https://docs.docker.com/engine/reference/builder/) to help with deployment.

## Other Pre-Requisites to Consider
### Using Replit and ecnountering outdated docs
Replit has been updated and is not 1:1 with documentation on Battlesnake "Read the Docs". Here are a few things that you may have to consider to have a smooth set up and to run the game from Replit:
* The Starter Project Template for python button on the Battlesnake docs creates a GitHub repo and not a Replit. I was able to create a Replit after the repo was created using the button above. Also, Replit may cost money to use.
* When using Replit in the current version, the main.py and other files are not automatically open. You have to search for the files by using the magnifying glass in the top right corner. The starter kit files will be visible to choose from in the list.
* Webview is now called Preview in Replit. You can search for the Preview module in Replit and then drag the tab anywhere in viewer to have a split screen between files and outputs. 
* Once you press the green arrow to run 'main.py', it will then generate the URL needed in the preview module when creating a battlesnake in the "My Battlesnakes" section on play.battlesnake.com. The URL may possibly look like a long series of numbers, dashes, and letters but should end with '.replit.dev'. Only after this will you be able to create a game.

### Virtual Environment
Whether you're using developing using your local computer through GitHub there are a pre-reqs needed when using Flask in a virtual environment.

## Run Your Battlesnake

Install dependencies using pip

```sh
pip install -r requirements.txt
```

Start your Battlesnake

```sh
python main.py
```

You should see the following output once it is running

```sh
Running your Battlesnake at http://0.0.0.0:8000
 * Serving Flask app 'My Battlesnake'
 * Debug mode: off
```

Open [localhost:8000](http://localhost:8000) in your browser and you should see

```json
{"apiversion":"1","author":"","color":"#888888","head":"default","tail":"default"}
```

## Play a Game Locally

Install the [Battlesnake CLI](https://github.com/BattlesnakeOfficial/rules/tree/main/cli)
* You can [download compiled binaries here](https://github.com/BattlesnakeOfficial/rules/releases)
* or [install as a go package](https://github.com/BattlesnakeOfficial/rules/tree/main/cli#installation) (requires Go 1.18 or higher)

Command to run a local game

```sh
battlesnake play -W 11 -H 11 --name 'Python Starter Project' --url http://localhost:8000 -g solo --browser
```

## Next Steps

Continue with the [Battlesnake Quickstart Guide](https://docs.battlesnake.com/quickstart) to customize and improve your Battlesnake's behavior.

**Note:** To play games on [play.battlesnake.com](https://play.battlesnake.com) you'll need to deploy your Battlesnake to a live web server OR use a port forwarding tool like [ngrok](https://ngrok.com/) to access your server locally.
