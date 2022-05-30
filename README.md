<p align="center">
  <a href="https://aoi.js.org">
    <img width="400" src="https://github.com/aoijs/website/blob/master/assets/images/aoijs-new.png?raw=true">
  </a>
</p>

<h1 align="center">aoi.js</h1>

<div align="center">

**The most advanced package to create a Discord Bot fast and powerful.**
    
[![NPM version][npm-image]][npm-url]
[![AoiJS Server][aoijs-server]][aoijs-server-url]
[![NPM downloads][download-image]][download-url]

The replacement of [dbd.js](https://www.npmjs.com/package/dbd.js)

[npm-image]: http://img.shields.io/npm/v/aoi.js.svg?style=flat-square
[npm-url]: http://npmjs.org/package/aoi.js
[download-image]: https://img.shields.io/npm/dt/aoi.js.svg?style=flat-square
[download-url]: https://npmjs.org/package/aoi.js
[aoijs-server]: https://img.shields.io/discord/773352845738115102?color=5865F2&logo=discord&logoColor=white
[aoijs-server-url]: https://aoi.js.org/invite
    
</div>

## Features

- Built-in support of [database](https://www.npmjs.com/package/dbdjs.db) by default and ready for multipurposes.
- Built-in 500+ functions, simple and easy to learn.
- Simple to learn, all in string based and compact.
- Support of extensions available to be used by the community.

## Installation

**node.js 16.6.0 or newer is required.**  


```bash
npm install aoi.js
```

```bash
yarn add aoi.js
```

## Setup

```js
const aoijs = require("aoi.js")

const bot = new aoijs.Bot({
token: "DISCORD BOT TOKEN",
prefix: "DISCORD BOT PREFIX",
intents: ["GUILDS", "GUILD_MESSAGES"]
})

//Events
bot.onMessage()

//Command Example (ping)
bot.command({
name: "ping",
code: `Pong! $pingms`
})

//Ready Event
bot.readyCommand({
    channel: "",
    code: `$log[Ready on $userTag[$clientID]]`
})
```

## Function usage Example

```php
$authorID - Return the author ID/the userID who executed the function
```

## How does it work?

It fairly simple, by using `$` as a sense of a function to execute per say it's run by a command.
By using `$` after the function name, and it's addtional fields, (if any) it'll work as intended by it function 

### Optional Extensions

- [@akarui/aoi.music](https://www.npmjs.com/package/@akarui/aoi.music) to enable Music Functions compatibility. (`npm install @akarui/aoi.music`)
    
## Links
- [Website](https://aoi.js.org)
- [NPM](https://www.npmjs.com/package/aoi.js)
- [Github](https://github.com/AkaruiDevelopment/aoi.js)
- [Discord Support Server](https://discord.gg/HMUfMXDQsV)
- [Documentation](https://akarui.leref.ga/v/aoi.js/)
