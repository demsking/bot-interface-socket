# bot-interface-socket

A socket interface for your bot (ibot)

## Install

```sh
npm install --save bot-interface-socket
```

## Usage

```js
const iSocket = require('bot-interface-socket')
const bot = require('./lib/your-ibot')

bot.configure({
    interface: iSocket
})

process.on('SIGINT', () => {
    bot.exit()
    process.exit()
});

bot.run()
```

## License

Under the MIT license. See [LICENSE](https://github.com/demsking/bot-interface-socket/blob/master/LICENSE) file for more details.
