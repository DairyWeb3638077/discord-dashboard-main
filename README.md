<img src="https://i.imgur.com/1JEnQ5p.png" width="650" height="auto">

# Discord Dashboard Example

A simple Discord Bot Dashboard that is coded with Express, MongoDB and Discord.js

**Screenshots:** [Click Here](https://imgur.com/a/LJTHT3j)

## Requirements

- Node.js **v17** or later
- Discord.js **v13.6.0** or later

## Setup

1. Create a Discord Application and name it.

![alt text](https://i.imgur.com/luHPTGL.png "Step 2")

2. Rename `example.env` to `.env` and fill the required values from the Discord **OAuth2** and **Bot** Page. **Do not show anyone these!**

3. Install all of the required NPM modules with the following command...

```bash
npm install --save
```

4. Add the callback URL to the Bot's **OAuth2** Page. Click the save button after that.

![alt text](https://i.imgur.com/9EWhEnE.png "Step 3")

5. Create a MongoDB database. You can choose between hosting it yourself (locally, VPS) or from [MongoDB Atlas](https://www.mongodb.com/atlas/database). Then paste the connection string into the `.env` file. The connection string is in the format of `mongodb://<username>:<password>@<host>:<port>/<database>`. (Might be different!)

6. After filling out the `.env` file, run the following command in the console to deploy the bot commands. This may take up to an hour to process through. Do this once unless you have made major changes to the commands (New Command, changed subcommands, etc).

```bash
npm run deploy
```

7. Start the dashboard.

```bash
node bot
```
