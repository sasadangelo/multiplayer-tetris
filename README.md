Multiplayer Tetris
======

* Classical Tetris type of game
* Multiplayer feature
* Live updates/broadcast of all players playing
* Highscores

Demo [here](https://multiplayertetris.eu-gb.mybluemix.net/)

Development/Setup
-----
Dependencies for the Server (npm)
```
    cd \<work directory\>
    git clone https://github.com/sasadangelo/multiplayer-tetris.git
    cd multiplayer-tetris
    npm install
```

To start the Server:
```
    npm start
```

Point Browser to: `http://localhost:6003` (when server starts it shows the exact URL to put in the browser address bar), enter a name and play or watch others currently playing - live.


Play [here](https://multiplayertetris.eu-gb.mybluemix.net/)


# How to deploy Tetris on IBM Cloud

In order to show you how to deploy your first application on IBM I cloned this Node.js project from this [repository](https://github.com/zhongdeliu/multiplayer-tetris). It is a Tetris multiplayer game you can run on web. I moved the code in the public folder and added some files required for IBM Cloud integration.

## Instructions to deploy Multiplayer Tetris on IBM Cloud

1. Create an account on [IBM Cloud](https://www.ibm.com/cloud/). For demo purpose you can use the *Lite* pricing model that  
   allow you to work for free. The limit is that the application will be removed after 10 days on development inactivity. On 
   *Lite* pricing model you cannot choice a region different by the one associated to the default space of your account.  
2. Use "MultiplayerTetris" as application name, "multiplayertetris" as host name. Domain, region, organization and space are set by 
   default. Press the Create button.
3. Download and install IBM Cloud CLI as explained [here](https://cloud.ibm.com/docs/cli/index.html#overview).
4. cd \<work directory\>
5. git clone https://github.com/sasadangelo/multiplayer-tetris.git
6. cd \<work directory\>/multiplayer-tetris
7. bluemix api https://api.<region\>.bluemix.net

   where \<region\> is:
   - ng, for Dallas;
   - eu-gb, for London;
   - eu-de, for Frankfurt;
   - au-syd, for Sydney;
   - us-east, for Washington;
       
8. bluemix login -u \<your email\> -o \<organization\> -s \<space\>       
9. bluemix app push MultiplayerTetris

You can see the MultiplayerTetris demo [here](https://multiplayertetris.eu-gb.mybluemix.net/).
