# $djsEval

This function evals the given discord.js code

> ❗ You should restrict the use of this function to yourself

#### Fields

This function has 1 required field

1. Code \(Required\)
2. Return Code \(Optional\)

Raw Usage: `$djsEval[code;return code (yes/no) (optional)]`

#### Options

* Code - The discord.js code we're evaling
* Return Code - Returns the output of the code without message.channel.send\(...\)

#### Usage

Evaling a pre-written code

```javascript
bot.command({
name: "eval",
code: `
$djsEval[
for(let i=0;i<10;i++) {
message.channel.send('hello')
}
]
`
})
```

Evaling the user's message

```javascript
bot.command({
name: "eval",
code: `
$djsEval[$message]
`
})
```

With the optional field

```javascript
bot.command({
name: "eval",
code: `
$djsEval[let a = 'apple'
a;yes]
`
//Will return 'apple' without m.channel.send(...)
})
```



