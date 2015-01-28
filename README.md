# Twitch Polls

This is a nwjs app that you can use to run polls in Twitch Chat and display those results live on your stream.

## Installation

There is no installing, just download the release package, unrar the file, and run TwitchPolls.exe

## Running a Poll

Running a poll is simple, just choose your poll type, duration, and type in your question. If you use a custom poll type you also have to enter your poll options.

Then simply hit "Start Poll" to start the poll in twitch chat. The program will send a message to twitch chat (under your username) asking people to respond to the poll, and when finished will publish the poll results into twitch chat. You can also hide the results from twitch chat by changing the "Show Results" option.

## Integrating into stream

You can integrate the results of the poll into the stream by adding the provided export url to your preferred stream tool's webpage plugin.

The results of the page are updated in real time as the poll is run. You can customize the output of the poll page by changing the file in `templates/results.html`.

The template file is a simple swig template, and all the available variables are described in the file.