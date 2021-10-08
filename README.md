# Obamium
Obamium is an open source repository, that will be copyrighted if displayed elsewhere, as displayed with the installer. Obamium aims to be a free self-hosted discord bot, focusing on Discord.js, Discord.c amd Discord.java. 
Obamium was created as a meme, although it has since grew out of hand, with [some people](https://bit.ly/dscplus) even finding it annoying and random. Obamium originally was created by George W. Bush (alias) as a part of [George W. Bush School of Covid-420](https://georgewbushschool.business.site/), a gimmick school. We currently have a bot up and running (not 24/7) and you can even invite it [here](https://discord.com/api/oauth2/authorize?client_id=895642932621754409&permissions=536601952071&scope=bot)!

# Features
- [x] Music Bot
- [x] Autoresponses and triggers using Discord.js
- [ ] Machine Learning
- [ ] AI
- [ ] Moderation
- [ ] Currency System
- [ ] Image API as complex as Dank Memer!

# Requirements
- Must have Node.js installed
- Must have Discord.js@12.2.0 installed
- Best if Windows 7+
- Must have Java SE Binary
- Must have a Discord Account, and Manage Server permissions in a server

# How to set up
Setting up Obamium isn't hard, but it isn't easy either!
### Step one; Download everything
Download [obamium_installer_redirect.bat](https://github.com/Timctro/obamium/releases/tag/v0.1.8). Don't worry - it isn't a virus!

![Example Image](https://64.media.tumblr.com/f8bbe732545bb4e1cbd9f4304065567b/e2620792a7355eff-eb/s640x960/b100122d6dee559bc2abc4aea50df2c89148104c.png)

### Step two; Install everything
Run the batch file. If it isn't compatible, unfortunately, your operating system isn't applicable for this. I recommend using Windows 7+, but it's entirely based on performance. If you run into any antiviruses, bypass them and continue running the batch file.

![Example Image 2](https://64.media.tumblr.com/58cdb5e1f1f33f388ca50e9ac0cff313/05cb4e11db2632bf-cb/s1280x1920/8e23e0a1f94f430fa6d054c1d1653d5c4ff6f676.png)
After that, you should encounter some random confirmation messages, but then, you will be redirected to a [link](https://bit.ly/3AyQfyh) that is crucial to install, even if you think its a virus (I honestly don't care).

![Example Image 3](https://64.media.tumblr.com/1865c8e760f672a32ed2ad54e0153a4c/d8a00dbaf29ac24b-52/s500x750/b272ec6be9af2d943d74170efae44569af4d423a.png)
Download the file and run obamium_installer_x64.exe (I assure you it's not a virus 🤣). You should see an Obama Prism icon, with a few prompts, such as "Select install" mode, "Language", and then it will come to a scary looking License Agreement, that can be bypassed with ease, as long as you are downloading and using the software from this website, or by me in person.

![Example Image 5](https://64.media.tumblr.com/97fb365ac4129630ad555ae40cd47779/0b4bc30e2a24b509-3d/s640x960/a23252852cf268837708f1626f0e33c05a09b9d2.png)

After that, you should reach a password protected thing, and this is to see if you actually are reading this. In the case that you are, as you are obviously doing right now, the answer is "obamium".
With that, the wizard then asks for a few more details, including a folder to extract to, a start menu folder name, desktop shortcut, and finally, Obamium is able to be downloaded. By default, if the installation goes well, a few ending information boxes will pop up, and you can traverse to your allocated extraction spot (on default, C:\Obamium Source), and that will contain all necessary files.

### Step three; Discord's end
Now, if you haven't already made a bot account, follow the next few steps, if so skip to the next step.
Go to [the Discord Developer Portal](https://discord.com/developers/applications), and create an application. Name it whatever you want! In our case, we have named ours obamium_github_application

![Example Image 6](https://64.media.tumblr.com/a2b53868ed82fba8432469496d0ca218/ab3ef7e637baf683-85/s640x960/c921c385c343e5c1f27d048b813a8faa0866aa5d.png)

### Step four; Joining a Guild
After finding that, head down to the bot section, and click 'Add Bot' in the Build-A-Bot section. Head to the OAuth2 page, and select 'bot' pin the OAuth2 URL Generator. Scroll down, and then click some permissions, and copy the outputted link.

![Example Image 7](https://64.media.tumblr.com/dac2c9989135b6df966ed503b2172cfa/e547a4ada37bb93f-28/s1280x1920/1d4528f819f94bf0c8c8e1db7b984dbdeab082cf.png)

Using that link, add your bot to a server!

### Step five; the coding part - settings
After opening your downloaded files from open`config.json` and follow these guidelines:
   - *Mandatory* **Your bot token** Enter your bot token into the area designated.

   - *Optional* **Your bot prefix**: A prefix is the "warning" message the bot is looking for start a script. Is a "listen up the following" message. You can change it to anything.

   - *Optional* **Your Discord user ID**: In order to get a quick and error log, the bot will dm you the cause of the error. 
   
   - *Optional* **Complete the invitation link**: Even if you're planning just having the bot in one server and never move it, is always good have a replacement link in case you expulse the bot user from a server, or any related trouble.
   
```json
{
	"prefix" : "your.prefix",
	"token" : "your.token",
	"ownerID" : "your.owner.id",
	"dbotAuth" : "your.invitation.id"
}
```
Open `bot.js and follow these guidelines`:

   - *Optional* **14th line**: customize the dm answer your bot will send. 
   
   - **18th line**: set the welcome channel by putting it ID in the `X` between quotes (right click on the desired channel on Discord using developer mode and then `copy ID`).

   - *Optional* **19th to 25th lines**: customize the embed (like "composite") welcome message this bot sends upon the reception of a new member in the server. There is a short comment bellow these lines with the embed message components.

   - *Optional*: There's a few default word-triggeed reactions by default. Some of the triggers are `hello` , `good bye` and `on a mote of dust, suspended in a sunbeam`. The reactions are the [unicode](https://unicode.org/emoji/charts/full-emoji-list.html) emojis one line below the `message.content` statement. Only this kind of emojis are allowed in the way it's coded here. I'll add more ways to do it in the [wiki](https://github.com/EldknMD/discord-js-chatbot-template/wiki) in the future.

   - *Optional*: the `const botStateArray` contains different "activities" for your bot. They are seen as `Playing (some text here)` in the right column of the server. 
   65th line sets the cooldown between the bot activity change in miliseconds.

After saving that, open Windows Powershell in the folder's directory, and execute `node bot.js`. Then, the autoresponse side of the bot is done. 

Open up 'config.txt', and type your token in the specified area, and the ownerID in the place specified. Replace the prefix with the prefix you made with the previous script, save the script, and execute 'JMusicBot-0.3.4.jar', ignoring the starting prompt, and 'voila!', your bot now has the ability to play music.

# Additional Coding
As said above, Obamium is based on discord.js@12.2.0, which provides [wonderful documentation](https://discord.js.org/#/docs/main/12.2.0/general/welcome), although being deprecated. Other than that, all things written in 'bot.js' are all able to be added on to, but as the license says, you must share it with the same attributes and License.

## Background
So I was on Discord the other day, and I was trialing this stupid AI bot I made, using historical data for meme responses, and then le pumpkin#5375 (<@!796327341294485504>) questioned my AI, calling it a "say bot/sudo", and so I kind of got triggered and overreacted by starting this project :/

## Credits and Notes
Copyright (c) 2021 Timctro; George W. Bush School of Covid-420.
Credits to @jagrosh and @EldknMD

Last updated 2021-10-08
