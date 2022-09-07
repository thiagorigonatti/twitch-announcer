# twitch-announcer
A bot to announce in a discord server that you are live-streaming to twitch

[![](https://img.shields.io/discord/677642178083946580?color=%23768ACF&label=Discord)](https://discord.gg/U8NcPcHxW3) [![Twitch Status](https://img.shields.io/twitch/status/thiagorigonatti?label=Twitch)](https://twitch.tv/thiagorigonatti)
[![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/subscribers/UCEDjQf5cEkH4320GevAitUA?label=Thiago%20Rigonatti)](https://www.youtube.com/thiagorigonatti)
[![](https://img.shields.io/badge/Linked-In-blue)](https://www.linkedin.com/in/thiagorigonatti/)
[![](https://img.shields.io/badge/Udemy-2%20Courses-blueviolet)](https://www.udemy.com/user/thiago-rigonatti-2/)

<img align="right" src="https://cdn.discordapp.com/attachments/1000867656267739207/1023941472195719258/twitch-announcer.png" height="256"></img>

# TwitchAnnouncer (Discord bot)

1. [Introduction](#twitchannouncer-discord-bot)
2. [How to](#how-to)
3. [Command usage](#Commands)
4. [Notes](#Behavior)
5. [Sample](#Sample)

## How-to
[TwitchAnnouncer](#TwitchAnnouncer (Discord bot)) is a [Discord](https://discord.com/) bot made with [JDA](https://github.com/DV8FromTheWorld/JDA) which allows you to configure a running task that its mission is notify the role set whenever the twitch account set goes online; it will send an embed message to the subscribed message channels to perform the notification.

To introduce [TwitchAnnouncer](#TwitchAnnouncer) bot in your discord server, use the following link:
[Invite](https://discord.com/api/oauth2/authorize?client_id=999699275221061773&permissions=150528&scope=bot%20applications.commands)

## Commands
*NOTE: You must to have MANAGER_SERVER permission in order to use these commands*

`/setlang <lang>`
**Defines the default bot language in the server.**

`/subscribe <streamer_login> <role> #<lang> #<locale> #<timezone>`
**Subscribes a streamer to be announcing your live-streaming and mention the supplied role; note that if lang, locale or timezone is not passed so this announce will use the server ones.**

`/unsubscribe <streamer_login>`
**Unsubscribes a streamer, cancel the announcement for the channel.**

## Behavior
The bot status will keep changing to show all subscribed streamers in its status as `streaming: streamer` and a clicable link button to it.

If you subscribe an already subscribed streamer in the same channel, it will overwrite the options that you have supplied.

The bot must be allowed in the message channel to send the notification message.

#### Sample
<img src="https://cdn.discordapp.com/attachments/1000867656267739207/1002672392163831808/notification-sample.png"></img>