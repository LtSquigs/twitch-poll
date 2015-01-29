# Twitch Polls

This is a Windows Application that you can use to poll Twitch viewers in twitch chat and integrate those results into your live streams.

## Installation

Installation of Twitch Polls, simply [download the release rar](https://github.com/LtSquigs/twitch-poll/releases/download/1.0.0/TwitchPolls.rar), extract the rar somewhere, and run TwitchPolls.exe in the extracted directory.

## Creating a Poll

Creating a poll is easy, all you have to do is set the poll options and then start the poll.

The options that you can set are as follows:

* **Poll Duration** - The duration the poll runs
* **Show Results In Chat** - If turned on the results of the poll will be published in chat when finished, otherwise only a simple "Poll Finished" notification will be published to chat.
* **Poll Type** - The type of poll you want to run, including Custom polls where you can create any kind of poll you want.
* **Question** - The Question the poll is asking
* **Options** - If using a custom poll, you must fill out the options that users may vote for.

After you've set the options you want, you just have to hit the "Start Poll" button to start the poll. The application will send a message to the chat (under your channels username) signifying the start of the poll and describing how to vote for the various options.

The poll will run for the duration set in the options, then when finished will display the results based off of your settings.

## Integrating into stream

You can integrate the results of the poll into your stream by simply adding the URL provided as an "Export Url" to the scene in your streaming software. For XSplit 2.0 you can add this directly as a Webpage URL, for OBS you may need to load the page in a web browser and include the browsers tab.

The "Export Styles" option lets you change some of the details of how this information is output, including the background color (for chroma keying), the text color, and how large the text is. 

For more detailed changing of the exported web page, go to the "Changing the results page" section of the readme.

The default settings are optimized for XSplit which automatically sets the background of the page to transparent. For OBS you may need to change the background to a color you can Chroma Key out.

## Changing the results page

The default results page is designed to give you a spartan set of results that you can easily change through custom CSS or JS in XSplit.

However, if you need a different layout to fit your stream you can easily change how the webpage outputs by changing the `templates/results.html` file.

This file is a [simple swig file](http://paularmstrong.github.io/swig/docs/#variables) with all of the various variables and things you may need to create the exact layout you want documented in the file itself.
