# Twitch Plays Robotics (TPR), minimal installation.

## Set up a Twitch Channel.

1. Create a Twitch.tv account at www.twitch.tv if you do not already have one.

2. Obtain your stream key as explained at https://youtu.be/g-cPiO73ReU

3. Never expose this key to your viewers, but if it does occur, change the key!

4. Download, install, and run Open Broadcaster Software (OBS) from https://obsproject.com/

5. Connect OBS to your Twitch account as explained at https://youtu.be/a7L3o5E0bak

6. Launch OBS and click "start streaming" (which will stream to your twitch channel).

## Set up a chat bot.

1. You now need to create a chat bot that will collect the text that your users type into your Twitch channel.

2. Create a second Twitch account using the name of your bot. It can be called anything you like.

3. Obtain an oauth token for your chat bot as explained at http://www.twitchapps.com/tmi/.

4. Login in to your chat bot's twitch account, and copy the generated token.

5. Edit settings.py with your Twitch information: 

```
CHANNEL=name of channel you want to stream,
IDENT=name of the twitch account acts as a chat bot,
OAUTH=oauth token obtained from the previous step.
```

6. Run "python chat_bot.py" to activate your chat bot.

