# How to get your Minecraft bearer token

## What is a Minecraft bearer token?

A bearer token is a long string of letters and numbers used to authenticate your account with their private API.

## Get your bearer token

1. Sign in to your Minecraft account at [minecraft.net](https://minecraft.net)
2. open the chrome / firefox dev tools (ctrl + shift + i) _or_ right click and click inspect
3. Go to the "console" tab
4. paste this code into the console:
```js
console.log(`; ${document.cookie}\`.split(`; bearer_token=`).pop().split(';').shift())
```
6. copy the bearer token that it shows in the console

You now have your minecraft account's bearer token.

**IMPORTANT: if you give someone this token they basically have full control of your minecraft account. They could change the password.**
