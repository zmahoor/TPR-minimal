----------------------------TO SET UP A TWITCH CHANNEL--------------------------
1. Create a Twitch.tv account at www.twitch.tv if you do not already have one.

2. Obtain your stream key as explained at https://youtu.be/g-cPiO73ReU

3. Never expose this key to your viewers, but if it does occur, change the key!

4. Set up Open Broadcaster Software (OBS). You need to connect OBS to your twitch account
 created in the previous step. 

	-Download from https://obsproject.com/download
	-Enter twitch channel information
	-More info:
		+https://github.com/jp9000/obs-studio/wiki/OBS-Studio-Overview#quickstart
		+https://help.twitch.tv/customer/portal/articles/1262922-open-broadcaster-software

3. Launch OBS and click of "start streaming" (which will stream to your twitch channel).


----------------------------TO SET UP A CHAT BOT(optional)--------------------
1. Make another Twitch account that acts as a chat bot which connects to your streaming channel and read messages from/to the chat panel.

2. To obtain an oauth token for a twitch account that serves as a chat bot: 

      Click http://www.twitchapps.com/tmi/ and login in to your twitch account that is supposed to be a chat bot, then copy the generated token. 

3. Edit settings.py with your Twitch information: 
		CHANNEL=name of channel you want to stream, IDENT=name of the twitch account acts as a chat bot, OAUTH=oauth token obtained from the previous step.

4. Run "python chat_bot.py" to read messages entered into the chat section of your channel.
