# $slowmode

This function sets a cooldown to the given channel ID. `0` will set the cooldown to none

```text
$slowmode[channelID;time/0]
```

> ❗ Discord does not allow you to go over 6 hours

```javascript
bot.command({
name: "slowmode",
code: `Set the channel slowmode
$slowmode[$channelID;5m]` //Sets the current channel slowmode to 5 minutes
})
```

