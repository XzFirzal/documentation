# bot.musicEndCommand

#### Usage:

```javascript
bot.musicEndCommand({ //Command
channel: "channel", //Channel where the logs are going
code: `your code` //Code
})
```

#### Example Command:

This command triggers everytime the music playback ends in a server. [$channelID](functions/usdchannelid.md) is where the play song command was executed.

```javascript
bot.musicEndCommand({ 
channel: "$channelID", 
code: `The music queue ended!` 
})
```

