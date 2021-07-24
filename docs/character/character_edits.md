# Character Edits

## Manually mark a quest as complete

1. Find the quest ID for the quest you want to change from the [quests directory](../resources/quests/).
2. Open the `JET/Server/user/profiles/{AID}/character.json` file with a decent text editor. 
3. Search the file for your quest ID.
4. Look for your quest's `status` property. It will usually say `"status": "Success"` or `"status": "Started"`.
5. Change the value to `AvailableForFinish`. It should now say `"status": "AvailableForFinish"`. The quest can now be submitted.
    - If, in the raid, you were killed with a quest item, and it no longer spawns on the map, you can change the value to `AvailableForStart` to take the quest again.
    
## Modify XP Rate

1. Navigate to `JET/Server/db/cacheBase/globals.json`. Be careful when editing db/ files.
2. Search for the `SkillProgressRate` and `WeaponSkillProgressRate` properties.
3. Set these properties to `1` for a live-like rate, or to whatever you want.
4. Save and clear your user cache.

## Change your roubles amount

<iframe width="560" height="315" src="https://www.youtube.com/embed/MJYykF2lm6k" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**NOTE:** Make sure you set the value of roubles to a number below a 32-bit signed integer's max value (2.147 billion). If you don't, anything involving money will fail to process in-game. We usually recommend 999 million.

*Courtesy of Raven*

## Modify your trader standings

<iframe width="560" height="315" src="https://www.youtube.com/embed/Yk6fkZqaO6U" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

*Courtesy of Raven*

## Modify your character's level

<iframe width="560" height="315" src="https://www.youtube.com/embed/-im_c2c_MW0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

*Courtesy of Raven*

## Modify your character's skills

<iframe width="560" height="315" src="https://www.youtube.com/embed/fyHzYhCoAeI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

*Courtesy of Raven*
