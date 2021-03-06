# liri-node-app

LIRI stands for *Language Interpretation and Recognition Interface*.
LIRI makes use of JavaScript, Node.js and various packages to take in user input from the command line. It uses API calls for Spotify, IMDB (Internet Movie DataBase), and Bands in Town, as well as a custom query that extracts data from a text file and outputs the results to the command line/console.

## Setup:
1. If not installed already, download & install **`Node.js`** on your computer: https://nodejs.org/en/

2. Copy the files to the directory you wish to run LIRI from. You will only need to copy the following files: `keys.js, liri.js, package-lock.json, package.json`, and `random.txt`. The gifs and images folders are for the readme file.  
3. To use the Spotify functionality, you will need to get a **`Spotify ID`** and **`secret`**.

    a. Visit <https://developer.spotify.com/my-applications/#!/>
    
    b. Either login to your existing Spotify account or create a new one (a free account will work) and log in.
    
    c. Once logged in, navigate to <https://developer.spotify.com/my-applications/#!/applications/create> to register a new application to be used with the Spotify API. You can fill in whatever you'd like for these fields. When finished, click the **`complete`** button.
    
    d. On the next screen, scroll down to where you see your client id and client secret. Copy these values down.
    
    e. Create a new file named **`.env`** in the same directory as the other files you created and paste in the following, each item on its own line. Replacing the code after the = sign with your Spotify ID and secret.

    **`SPOTIFY_ID=your-spotify-id`**

    **`SPOTIFY_SECRET=your-spotify-secret`**

    create the .env file highlighted here:

    ![LIRI directory structure](./images/directory_structure.png
    )

4. At the command line in the directory where the LIRI files are located, type **`npm i`** - this will read the **`package.json`** file and install any packages needed by LIRI. They will be installed in the node_modules folder.


## How to use LIRI:
To use this app, navigate in the command line to the directory where the LIRI files are located, type **`node liri`**, and enter 2 items: 
* for concert info, type **`concert-this`**, followed by the artist you want to search.
* For spotify info, type **`spotify-this-song`**, followed by the artist name. 
* For movie info, type **`movie-this`**, followed by the movie title. 
* Entering **`do-what-it-says`** processes the output from an existing text file, random.txt. 

Note: For elements with more than 1 word in their name, surround the content in quotes.

For example - type this at the command line: **`node liri movie-this "Star Wars"`**

For help in the console, type **`node liri help`**

### LIRI-help
![LIRI help](./images/liri_help.png)

## Demo

### LIRI concert-this 
![LIRI concert-this](./gifs/liri-concert-this.gif)

### LIRI spotify-this-song 
![LIRI spotify-this-song](./gifs/liri-spotify-this-song.gif)

### LIRI movie-this 
![LIRI movie-this](./gifs/liri-movie-this.gif)

### LIRI do-what-it-says 
![LIRI do-what-it-says](./gifs/liri-do-what-it-says.gif)

## Technologies used:
* JavaScript
* Node.js - https://nodejs.org
* Moment.js (for date formatting) - https://www.npmjs.com/package/moment
* Axios HTTP client - https://www.npmjs.com/package/axios
* Node Spotify API - https://www.npmjs.com/package/node-spotify-api
* dotenv (to access the .env file) - https://www.npmjs.com/package/dotenv


---
**LIRI** was coded by me, and is maintained by me.