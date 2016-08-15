# docker-discordpy-playlist

This is a complete docker image for discord.py's playlist.py example, with all dependencies included and ready to go. Use this to play music on a Discord server.

There have been slight modifications to add ENV-based configurables. These can be modified in the `docker-compose.yml` file.

# Requirements

* docker
* docker-compose

# Instructions

1. Get your own API token [here](https://discordapp.com/developers/applications/me) by creating an application.

2. Click 'Create a bot user' and confirm to get the right token. Copy the API bot token.

3. Open and edit docker-compose.yml.

4. Change TOKEN to your Discord application's API bot token. Preserve the quotes around your token.

5. Run with `docker-compose up` (to run in detached mode, run with `docker-compose up -d`)

Once the image is pulled and started, it will need to be joined to a Discord server. This uses the client ID, found on the applications page where the bot API token was.

1. Log into Discord normally.

2. Copy and paste this into a separate browser tab, swapping `CHANGE_ME` for your own client ID. https://discordapp.com/oauth2/authorize?client_id=CHANGE_ME&scope=bot&permissions=0

3. Load the page; Discord will prompt to add the bot to the server. Confirm and close.

4. Open the server that the bot was joined to, and look to see if the bot is online.

5. Start using it by sending `$help` in chat.

# Source reference

 https://github.com/Rapptz/discord.py/blob/master/examples/playlist.py

# License

See: https://github.com/Rapptz/discord.py/blob/master/LICENSE
