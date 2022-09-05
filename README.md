<img src="https://i.imgur.com/1JEnQ5p.png" width="650" height="auto">

# Discord Dashboard Example

A simple Discord Bot Dashboard that is coded with Express, MongoDB and Discord.js

**Screenshots:** [Click Here](https://imgur.com/a/LJTHT3j)

## Requirements

- Node.js **v17** or later
- Discord.js **v13.6.0** or later

## Setup
```bash
1. git clone https://github.com/DairyWeb3638077/discord-dashboard-main
```

2. Create a Discord Application and name it.

![alt text](https://i.imgur.com/luHPTGL.png "Step 2")

3. Rename `example.env` to `.env` and fill the required values from the Discord **OAuth2** and **Bot** Page. **Do not show anyone these!**

4. Install all of the required NPM modules with the following command...

```bash
npm install --save
```

5. Add the callback URL to the Bot's **OAuth2** Page. Click the save button after that.

![alt text](https://i.imgur.com/9EWhEnE.png "Step 3")

6. Create a MongoDB database. You can choose between hosting it yourself (locally, VPS) or from [MongoDB Atlas](https://www.mongodb.com/atlas/database). Then paste the connection string into the `.env` file. The connection string is in the format of `mongodb+srv://<username>:<password>@cluster0.oojpt.mongodb.net/<DB-NAME>?retryWrites=true&w=majority`. (Might be different!)

7. After filling out the `.env` file, run the following command in the console to deploy the bot commands. This may take up to an hour to process through. Do this once unless you have made major changes to the commands (New Command, changed subcommands, etc).

```bash
npm run deploy
```

8. Start the dashboard.

```bash
node bot
```
