# DC_Fortnite_Bot
A Fortnite bot for Discord

To use this bot you will need an account (I recommend an alt account) on the Epic Games Launcher,
Also you'll need to have Fortnite installed to obtain specific tokens.

[1] Install & Open Fiddler 4

[2] In Tools -> Options -> HTTPS, Select Capture HTTPS Connects

[3] In Tools -> Options -> HTTPS, Select Decrypt HTTPS traffic

[4] Start Capture (F12)

[5] After that start your epic games launcher.

[6] You will see a request with /account/api/oauth/token. Click on it and click after that on Inspectors get the header (Authorization header content and remove basic) => This header is your Client Launcher Token

[7] Press F12 to stop scan (Fortnite will stop working if you capture HTTPS requests at this moment)

[8] Launch Fortnite

[9] When the game tell you : "Connecting" or "Update" in waiting screen, Press F12 to reactivate requests capture

[10] You will see again a request with /account/api/oauth/token. Click on it and click after that on Inspectors get the header (Authorization header content and remove basic) => This header is your Fortnite Client Token

[11] Stop Capture

Configuration of the env file

    BOT_TOKEN= Your discord bot token.
	
    PREFIX= The prefix you would like to use for your bot.
	
    API_KEY= The api key that can be requested from https://fnbr.co
	
    EMAIL= Your fortnite account email.
	
    PASSWORD= Your fortnite account password.
	
    EPIC_API= [6]
	
    FORTNITE_API= [10]
	

The generation of the shop was done using https://fnbr.co though it broke,
You might want to look into how to fix it if you like.
