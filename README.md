[//]: #tech "Javascript,Discord.js"

<div style="
padding: 16px;
margin: 0;
border-radius: 6px;
background-color: #2f3136;
color: #606266;
font-weight: Bold;
width: 256px;
text-align: left;
font-family: monospace;
box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
margin-bottom: 32px;"
>Stats
<ul><li>Total Members: 524</li><li>Online: 41</li><li>Bots: 2</li></ul></div>

Discord bot, that can be linked with your server, for realtime member metrics in the channel bar.

## Config Format

Your `token` , target `server id` and `channel id's` need to be specified in `config.json`.
An empty template is already included.

**Note:** If you don't know your server ID, launch the bot just the `token`, to print some useful output.

###### Template

```json
{
  "token": "",
  "server": "342458782949875134",
  "totalChannel": {
    "id": "352314d718f4875f28",
    "name": "Total Members"
  },
  "onlineChannel": {
    "id": "369483985418813116",
    "name": "Online"
  },
  "botChannel": {
    "id": "345876991234719499",
    "name": "Bots"
  }
}
```

## Setup

1. Clone the repository with

```sh
git clone "https://github.com/volskaya/count"
```

2. Write down your server _ID_ and the _ID's_ of your server channels, in `json.conf`, that you wish the bot to update

- Total Members
- Online
- Bots

3. Open a shell in count directory and fetch node dependencies with `npm` from [Node](https://nodejs.org/)

```sh
npm update
```

4. Launch `main.js` with [Node](https://nodejs.org/)

```sh
node main.js
```

or

```sh
npm run bot
```
