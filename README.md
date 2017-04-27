# Twitch Plays Robotics (TPR), minimal installation.

----------------------------TO SET UP A TWITCH CHANNEL--------------------------
1. Create a Twitch.tv account at www.twitch.tv if you do not already have one.

2. Obtain your stream key as explained at https://youtu.be/g-cPiO73ReU

3. Never expose this key to your viewers, but if it does occur, change the key!

4. Download, install, and run Open Broadcaster Software (OBS) from https://obsproject.com/

5. Connect OBS to your Twitch account as explained at https://youtu.be/a7L3o5E0bak

6. Launch OBS and click "start streaming" (which will stream to your twitch channel).

----------------------------TO SET UP A CHAT BOT(optional)--------------------
1. Make another Twitch account that acts as a chat bot which connects to your streaming channel and read messages from/to the chat panel.

2. To obtain an oauth token for a twitch account that serves as a chat bot: 

      Click http://www.twitchapps.com/tmi/ and login in to your twitch account that is supposed to be a chat bot, then copy the generated token. 

3. Edit settings.py with your Twitch information: 
		CHANNEL=name of channel you want to stream, IDENT=name of the twitch account acts as a chat bot, OAUTH=oauth token obtained from the previous step.

4. Run "python chat_bot.py" to read messages entered into the chat section of your channel.
