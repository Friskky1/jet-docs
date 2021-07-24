# FAQ 

*This FAQ is pulled straight from the EmuTarkov Community Discord. It is recommended you join their Discord [here](https://discord.gg/NJANk5gCeN) for a more updated list.*

## What is this?
View [What is JustEmuTarkov?](https://docs.kiobu.dev/#what-is-justemutarkov).

## Will this get me banned from Tarkov?
As long as you’ve installed this separately from the live version and aren’t running BSG products to the side, until reported otherwise, this program should not cause any complications with your live account of Tarkov.

## How do I install this?
[Installation guide](/installation.md)

## I already have an old version installed, do I really have to install it all over again?
The binaries and server files are a small package, usually never exceeding 50 MB's. Sometimes, depending on how big the differences between versions are, a client patch will be manually compiled to at least try to cut down on data usage, however, the legality of this is yet to be proven, and are as such only provided as a service and can be withdrawn at any time.

## I already have Tarkov installed, can I use these files instead?
If the version of Tarkov live is the same as the version being used for JET, yes.
Simply copy all the client files to a separate folder, and extract the JET Binaries over them.
The JET launcher will delete and disable most unnecessary files automatically.

## I can’t find any copies of EFT, or, I can’t download them because of bandwidth limitations.
Although we may offer simpler compacted and stripped down versions to get the base program running, it is still advised that you purchase a copy of Tarkov from BSG and download the required files through their launcher instead. This Project was originated from a cheating forum and was made to make it easier to develop cheats for official game, where now its branched to allow players enjoy single player experiance. This project never was meant to be a PIRACY project and never will be. We are assuming that everyone who uses this project to play the game are already having game purchased. We dont have any way to detect if you have already purchased game or not, so we are unable check it in any respectable way to make sure that you have an official game bought.

## How do I give myself more money levels ect?
Most of the things you might want to modify has been well documented (with video examples) under [https://docs.justemutarkov.eu/](https://docs.justemutarkov.eu/)

## I changed some of the (gameplay) settings in the server files, but I don’t see the changes in game!
You might be required to clear your cache and restart the server to make it recache everything again. Remember to only edit files when the server is turned off, otherwise, changes may NOT be saved.

## How do I install mods?
You can usually install mods by extracting them into your Server\user\mods folder. After extracting your corresponding mod into its folder, usually said folder should contain some form of readme, or at least a file called ‘config.json’. You must be aware that mods must be esspecially created to the version of server you are using otherwise it will start crashing server or not work.

## I installed a mod and now my server stopped working!
Its almost 100% that mod you installed is not compatible with your version of the server, otherwise you extracted files wrongly. If you still have no idea how to fix it make sure to create support ticket on one of community discord's.

## Where do I change trader things?
Depends which exacly, if its player data of traders then in character.json (in user/profiles/YourId/character.json) otherwise it will be in database folder for traders (directory can change later on so i will not specify it but 100% it will be in folder DB)

## Where can I change my character’s data?
You can find most stats and such under your character.json, found under your server\user\profiles\YourId\character.json.  
You can also check this link [docs.justemutarkov.eu/character/character_edits/](https://docs.justemutarkov.eu/character/character_edits/)

## How do I give myself more money?
Simply visit this webpage and find what you are interested in [docs.justemutarkov.eu/character/character_edits/](https://docs.justemutarkov.eu/character/character_edits/)

## How do I increase the rate at which I gain XP?
you will need to edit database globals.json file for it. Inside that file find:  
`"skillProgressRate": 1`  
and:  
`"WeaponSkillProgressRate": 0.4`  
Change these to any rate you’d like.  
Those values are default EFT Live values.  

Tarkov has a skill fatigue system, which means that it will decrease the rate at which you gain skill points, the more you play.  
You will find a line in Globals.Json called ‘SkillFatiguePerPoint’, by default, the area looks like this:  
```
"SkillMinEffectiveness": 0.1,
"SkillFatiguePerPoint": 0.0006,
"SkillFreshEffectiveness": 1.3,
"SkillFreshPoints": 1,
"SkillPointsBeforeFatigue": 1000,
"SkillFatigueReset": 200,
```
Experiment with these values as you wish, lowering skillFatiguePerPoint, increasing skillMinEffectiveness and SkillPointsBeforeFatigue will all contribute to preventing fatigue from setting in, as well as increasing the amount of skillpoints you receive.

## How do I skip a quest?
A tutorial can be found here: [docs.justemutarkov.eu/character/character_edits/](https://docs.justemutarkov.eu/character/character_edits/)
Quest ID's can be found here: [docs.justemutarkov.eu/resources/quests/](https://docs.justemutarkov.eu/resources/quests/)
In your Character.json, you will find several mentions of “QID”. This stands for ‘Quest ID’. Example:
```
{
	"qid": "5eaaaa7c93afa0558f3b5a1c",
	"startTime": 0,
	"completedConditions": [],
	"statusTimers": {},
	"status": "Locked"
},
```
You can change the ‘Status’ of these to:
**“Locked”**
_Unavailable to start until requirements are met._
**“AvailableForStart”**
_Quest is ready to be activated. This can be handy to restart a quest, for example, when you lose a quest related item in a Raid._
**“Started”**
_Quest has been started and is waiting for all requirements to finish._
**“AvailableForFinish”**
_Quest can be delivered. Setting it to this allows you to collect the rewards._
**“Success”**
_Quest has been successfully completed, and rewards have been collected._


## How do I skip hideout progression?
In your character.json, you will find a section headlined “Hideout” your looking for the area "areas"
Each hideout item will look like this
```
{
	"type": 3,
	"level": 4,
	"active": true,
	"passiveBonusesEnabled": true,
	"completeTime": 0,
	"constructing": false,
	"slots": [],
	"lastRecipe": ""
},
```
here is a list of what each type is and there [docs.justemutarkov.eu/resources/hideout_areas/](https://docs.justemutarkov.eu/resources/hideout_areas/)  

## When I start the server, it crashes immediately!
First try deleting your cache, if that doesn't work then the server files are most likely corrupted, in that case copy your accounts.json and your character folders to a save place and re extract the server overriding everything in it, or simply delete server and reextract it in same place then reapply your accounts.json file and character profiles to not lose progression.

## I can’t extract when in a raid!
If this happends to you well thats a bad luck. You can use ALT+F4 to close game but rememebr progress wont be saved and you return to the state from before the raid.

## When I start the game, it tells me something about a key not being valid or not present, or, when I start, my stash is empty, I can’t access my hideout or my game won’t load into a raid!
The current version of JET has a Developer profile available, this is a leftover from the 12.8 version, and doesn’t work. You will have to make a new profile.

## The game is telling me it found some sort of Duplicate ID, and now it won’t load!
Have you installed the patch under Nr. 3 in #install ?
This fix will be implemented in future versions soon.

To repair your installation, you will need to manually clean your character.json. @Doctor has generously provided a bot that will do it for you! This file can be found under server\user\profiles\YourProfileID\character.json (server which holds this bot: [discord.gg/EmuTarkov](https://discord.gg/NJANk5gCeN))

Go to the "#bot" Channel. You will need to call it with !!clean, and attach your character.json file, an example can be found in "#announcements" channel

## My traders don’t work, are empty, or are stuck infinitely handling a transaction!
First, try clearing your server’s cache and restarting the server as demonstrated further above. If that doesn’t solve it, you may have an inconsistent item ID in your stash.
To confirm this, your CLIENT LOG (located in client\logs\date\date_traces.log) may contain something resembling the following:
```
EXCEPTION: System.ArgumentOutOfRangeException: Index and length must refer to a location within the string.
Parameter name: length
```
Normally, the ID will be mentioned in the related error, however, it most likely won’t display every item that has this problem.
In order to make sure all incorrect item IDs are eliminated, you will need to run the following patch using VSCode with node.js installed.
[check if over 24 patch](https://discord.com/channels/739984913599692881/739984972873596938/824837425528176650) from discord [discord.gg/EmuTarkov](https://discord.gg/NJANk5gCeN))

## What's the difference between JET (JustEmuTarkov) and the SPT-AKI project?
Both projects accomplish the same task. They both emulate the EFT backend server to allow you to play a singleplayer-only version of Escape From Tarkov. Intricately, both emulators have significant differences in code, but they are mostly indistinguishable for the user, as both function the same way. However, this means SPT-AKI mods will not work on JET, and vice-versa. Additionally, AKI requires a legitimate EFT license, whereas currently, JET does no legitimacy checks on the client. Most people make their choice based upon their perception of the communities or mod availability.

The major difference that separates SPT-AKI from JET is that JET has a small development team that is working to make a multiplayer-compatible JET server that allows you host a dedicated match server to play co-op with your friends. However, the development on this is very slow, considering the amount of reverse engineering required. Please don't ask us about the ETA for this, as it's a very ambitious project, and we work on it on our own time.

JET support is offered on this Discord, the partnered ConfigFreaks Discord, and the official JET Discord, whereas SPT-AKI support is only available on the Guilded known as Senko's Pub. We do not offer any support to SPT-AKI users, since there are major differences in code we have no idea about, and because this is a JET community, not an SPT-AKI one.

In case you're asking which one to choose, there's virtually no difference when it comes to performance, moddability, user friendliness, and quality of emulation. If you want the latest updates with possible bugs, SPT-AKI releases new updates quite frequently, and runs on a rolling release platform, where the latest game version is supported at the cost of potential instability. In contrast, JET works on a point-release system, where we release new updates relatively slowly to ensure as much stability possible. This means AKI may be a major version of EFT ahead, while JET would be on an older version.

## Where should I go if I want SPT-AKI support?
This is a JET Discord server. The official SPT-AKI developers are available on Guilded.gg on Senko's Pub. However, you can also receive AKI-related support on Discord at the EmuTarkov Related Community server [here](https://discord.gg/BpKdMkv).

Please note that EmuRC is not the official SPT-AKI community. They are an affiliate community, and as such have inherently different communities, structure, rules, staff teams, etc. Please be aware of this when intermingling between these communities.

## I have an issue/question about Altered Escape.
Because Altered Escape is a third-party mod for JET, and uses an experimental, in-development server build, we do not offer Altered Escape-specific support. You are best off looking for AE support [here](https://discord.gg/tagQAqw3HB).
