# CyberBot

A bot designed for the TIDB Future App Hackathon to solve both the issue of automated content moderation in discord voice channels and the language barriers that preside in a discord voice call.

# How to add to your server

1. Go to the discord developer web portal and create a discord bot

2. Copy the token in your computer's clipboard (Choose your app -> Settings -> Bot -> Build a Bot -> Copy Token)

3. https://discordjs.guide/preparations/adding-your-bot-to-servers.html#creating-and-using-your-invite-link has a very good explanation on how to do this.

4. Clone the git repository -> Either cloning the repo in github or in VSCode or other editors.

5. Add the token to a dedicated file. In our code, we have the tokens in config.json, under 'TOKEN'.

6. Open Ubuntu terminal and run this:
   `mysql --connect-timeout 15 -u '2rt95zELAjuaNfs.root' -h gateway01.eu-central-1.prod.aws.tidbcloud.com -P 4000 -D test --ssl-mode=VERIFY_IDENTITY --ssl-ca=/etc/ssl/certs/ca-certificates.crt -p(My Password What Is In TiDB)`

7. Open vscode terminal and run this: `$env:GOOGLE_APPLICATION_CREDENTIALS="Absolute/Path/To/Json"` (https://developers.google.com/workspace/guides/create-credentials) <- Follow this tutorial

8. In a terminal window in your code editor, run `npm i --force`

9. In the same terminal window, run `nodemon`

10. When running the code in discord (To run the translation code, it is /record, to run the detection code it is /detect, to change translation language go to constants and change the language code based on Google's language code)

# How to translate

To record, invite the bot to a discord server. In that server, type in /record in the designated bot channel (if any). A popup will appear showing a record and stop button. Once the clip is finished, hit stop.

# How to detect

To detect, invite the bot to a discord server. IN that server, type in /detect in the designated bot channel. A popup will appear shoing a record and stop button. Once clip is finisihed hit stop. In addition to configure "bad words" go to constants.

# Contact for help:

If any further instructions are required, please send an email to jeffqiu2025@crescentschool.org

# Functionalities

Can process all languages
Can auto-moderate voice channels

# Language Codes List

Google Language Code Website -> (https://developers.google.com/admin-sdk/directory/v1/languages)
