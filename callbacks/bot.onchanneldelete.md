# bot.onChannelDelete

This command gets triggered everytime a channel was deleted on a server.

#### Usage:

```javascript
bot.channelDeleteCommand({ //Command
channel: "channel ID", //Channel where its being logged
code: `your code` //Code sent to <channel>
})
```

#### Example Command:

```javascript
bot.channelDeleteCommand({ 
channel: "772414449839636490", 
code: `
Channel Deleted:
$oldChannel[name]
`
})
```

#### Options:

You can use the function [$oldChannel](functions/usdoldchannel.md) with the options below to return old channel data:

* `id` - The ID of the channel 
* `name` - The name of the channel 
* `topic` - The topic for this channel 
* `position` - The position of the channel 
* `categoryID` - The ID of the category this channel belongs to 
* `guildID` - The ID of the guild this channel belongs to 
* `lastMessageID` - The ID of the last message sent here \(if any\) 
* `type` - The type of this channel 
* `nsfw` - Whether the channel is nsfw or not 
* `slowmode` - The slow mode duration for this channel 
* `rawPosition` - The raw position for this channel 
* `deleted` - Whether the channel was deleted or not 
* `viewable` - Whether the channel was be seen by the client or not 
* `manageable` - Whether the client can or not manage this channel 
* `deleteable` - Whether this channel can be deleted by the client or not

