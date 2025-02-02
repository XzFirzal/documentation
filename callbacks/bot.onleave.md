# bot.onLeave

This callback that allows the bot to log every user who leaves the server.

```javascript
bot.leaveCommand({ //command
        channel: "channel id", //channel where the bot logs
        code: `your code` //Message sent to <channel>
})
```

> ❗ Make sure the &lt;channel&gt; is in the server. So recommended to use server variables \(if your bot isn't for 1 server\)

```javascript
bot.leaveCommand({ 
        channel: "782446718704812032", 
        code: `Goodbye, $username, hope you had a good stay at $serverName`
        /*
                Code Breakdown
        $serverName - The name of the server the user left
        $username - The user who left the server
        */
})
```

> ⚠ `GUILD_MEMBERS` intent needed! Information in the [Gateway Intents](guide/begin/gateway-intents.md) guide.

> ℹ️ You can use all guild and member based functions like [$serverName](functions/usdservername.md) or [$guildID](functions/usdguildid.md) or [$username](functions/usdusername.md) or [$authorID](functions/usdauthorid.md) in these commands.
