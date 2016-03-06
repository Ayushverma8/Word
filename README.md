# Word Search


I took every english word (over 200k words) and built a little NodeJS app that will help you find words that contain specific characters.

Additionally, here are instructions to deploy this app to Nodejitsu, Heroku, and Azure via Windows or Mac.

##How to Use

###The underscore

Type a word into the text box with the following pattern:

    he__o

And you'll get words such as:

    hello
    helio

###The question mark

This character is great for games like What's the Phrase (a knock off of Wheel of Fortune)

Type a word into the text box with the following pattern:

    st???

and you'll get words such as:

    stack
    stade
    staff
    stage
    stagy

but you wont get words like

    start

because the `t` would already be visible (in What's the Phrase), and you would have typed:

    st??t

##Instructions for running

Go to http://nodejs.org and install NodeJS

Then clone this repo:

    git clone https://github.com/Ayushverma8/Wordfinder.git

And `cd` into the directory (all instructions below assume you are in the `word-finder` directory:

    cd word-finder

##Run Locally

Install all the dependencies:

    npm install (you may need to prefix this with sudo if you're on Mac)

To run tests, type:

    jasmine-node .

If you want tests to execute every time you change a file:

    jasmine-node . --autotest --watch .

Run the app:

    node server.js

Then navigate to `http://localhost:3000`
