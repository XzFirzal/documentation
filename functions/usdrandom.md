# $random

This function returns a random number from the specified values

```text
$random[min;max;allowDecimals (yes/no);random (yes/no)]
```

```javascript
bot.command({
name:"random",
code:`$random[1;10;yes]`
//Returns a number between 1 and 10
})
```

