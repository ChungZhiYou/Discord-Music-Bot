# **Discord music bot**

## Available commands:
1. `/info` 
    
    Displays info about the currently playing song <br><br>
    
2. `/pause`
    
    Pauses the music <br><br>

3. `/play` *song's url*
    
    Loads a single song from a url <br><br>

4. `/play` *playlist's url*
    
    Loads a playlist of songs from a url <br><br>

5. `/play` *keyword(s)*
    
    Searches for song based on provided keywords <br><br>

6. `/queue`
    
    Displays the current song queue, optional to input page number, defaults to page 1 <br><br>

7. `/quit`
    
    Stops the bot and clears the queue <br><br>

8. `/resume`
    
    Resumes the music <br><br>

9. `/shuffle`
    
    Shuffles the queue <br><br>

10. `/skip`
    
    Skips the current song <br><br>

11. `/skipto` *track number*

    Skips to a certain track number <br><br>

***

## How to run:
Setup your own discord bot on the Developer Portal

    https://discord.com/developers/applications
Run npm packages installation

    npm init -y
    npm i dotenv discord.js discord-player @discordjs/voice @discordjs/rest @discordjs/opus @discordjs/builders

Create a file named `.env` which contains the token of the musicbot

    TOKEN = Insert_token_here

Include GuildID (server) and ClientID (musicbot) in the `index.js`

    const CLIENT_ID = "Insert_Client_ID_here"
    const GUILD_ID = "Insert_Guild_ID_here"

First run ***node index.js load*** to load slash commands into the bot

    $ node index.js load
    Deploying slash commands
    Successfully loaded

Then run the cmd ***node index.js*** to host the bot, ensure the terminal is occupied with this cmd to keep the bot active.

    $ node index.js
    Logged in as botName#ID