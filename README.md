# 🎵 PB-SubSounds 🎵  
  
This is a simple extension for Phantombot, allowing you to easily create user-specific sound alerts for Twitch subscribers or optionally for every user.  
  
**Why is this better than just using PBs built-in commands to trigger sounds?**  

✅ No need to create individual commands for every user. Keeps your command list clean.  
✅ One single command for everyone to use.  
✅ Multiple sounds per user are possible.  
✅ No additional setup. Just feed the bot with your sounds and it will handle the rest for you.  
  
  
## Get started  
  
1. Download from releases tab and drag the content of the zip file inside your phantombot directory. (includes english language file only)  
2. (Re)Start your bot.  
  
(3. Sub-Mode is enabled out of the box. To allow everyone, including non-subs, to use sounds, use the `**!togglesubsounds**` command.)  
  
The standard command to trigger SubSounds is `**!subsound**`. The command can be customized to your liking simply by creating an alias (like !hi).  
  
>⚠ I recommend to set a user-specific cooldown, so no one can spam their sound. (On the web panel go to `Commands -> Default -> !subsound -> >Edit`, change the cooldown value and untick the "Global" checkbox to apply the cooldown per-user)
  
### Get your sounds ready:  
This extension uses Phantombot's built-in audio hooks system, so you can drop the soundfiles where you normally would. Just make sure, that the filename of your soundfiles corresponds with the username they belong to.  
*Example:* Soundfile for user "MrKappa123" should be named `MrKappa123.mp3` or `mrkappa123.mp3` (Upper/Lowercase does not matter)  
  
### Assigning multiple sounds to a user:  
This can be easily done by adding a suffix to the soundfile's name. This suffix is also the command argument that's used to play that sound.  
*Example:* An additional soundfile for user "MrKappa123" can be named `MrKappa123_[YourSuffix].mp3` and the command would be `!subsound [YourSuffix]` or for the filename `MrKappa123_Scream.mp3` the command would be `!subsound scream`.  
