# Summer Collaborative Project


### How it will work:
Players will be able to create their own minigame that can be played in our Summer Collaborative Minigame map!
When you register your interest, you will be given a specific ID and string:
- Your ID will serve as both your plot number and your ‘minigame’ score number eg. "23"
- Your string will be the name that you should give to your dedicated function folder eg. "spleef"
When your minigame is selected to be ‘active’, a function will run a tick function within your folder (in this case, "spleef/tick"). This should be your primary method of activating commands. (If you need any help with this, you can always ask for help in the Bedrock Commands Community Discord!)

Your plot will be 96 blocks by 96 blocks. When you download the template world, you should run the command:

`/tag @s add ID{ID}`

This will lay out your plot where you can build. Please __do not__ build outside of these limits, only your 96x96 plot will be used in the final map.

### Using command blocks rather than functions
We 100% recommend that you get familiar with functions, they are much more performant than command blocks and can easily be versioned (so they don’t break if command syntax changes!) Now would be a great time to make the move; if you need help, other players on the project can help, we’re just a message away!

Nonetheless, if you do not want to use functions, then command blocks can be used, provided that the following execute command is places at the beginning of ALL of your command block chains:

`execute if score active minigame matches {ID} run …`

^ This makes sure your command blocks are toggleable with a score!

### Scoring System:
You are responsible for giving players the points they have earned from playing your minigame. These should be added to the scoreboard “points”. There are 2 different styles of point system:
- Podium: 1st Place gets 3 points, 2nd Place gets 2, 3rd Place gets 1
- Timed: All players who finish the minigame within the allocated time get 1 point!

### Things to note:
- Your plot will directly border another player’s plot; be considerate with blocks (eg. water, lava etc)
- Players will be in adventure mode, so if your minigame includes mining or placing blocks, you should use allow/deny blocks using the following commands:
```
/give @s allow
/give @s deny
```
- Structures ARE allowed, but make sure these are in a folder with your string name. (eg. ..structures/spleef/level_1; this would be given the structure name "spleef:level_1")
- Scripting will not be allowed due to the instability that they cause between versions.

### Queries
You are able to query if players have certain query properties, these are as follows:
| is_moving<br>is_moving_ground<br>is_alive<br>is_breathing<br>is_eating<br>is_first_person<br>is_gliding<br>is_in_water<br>is_invisible<br>is_jumping<br>is_on_ground<br>is_on_fire<br>is_riding<br>is_selected_item<br>is_using_item<br>is_sleeping<br>is_sneaking<br>is_sprinting<br>is_swimming<br>item_is_charged<br>last_hit_by_player | 2d_facing_north<br>2d_facing_east<br>2d_facing_south<br>2d_facing_west<br>3d_facing_north<br>3d_facing_east<br>3d_facing_south<br>3d_facing_west<br>3d_facing_up<br>3d_facing_down |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

Plus, health can be detected through the ‘health’ scoreboard

## TL;DR
- Registering: When you sign up, you'll receive a unique ID and a string. The ID serves as your plot number and minigame score. The string is the name for your function folder.
- Minigame Activation: When your minigame is selected to be active, a tick function will run within your folder. This function is responsible for activating commands in your minigame.
- Plot Size: Your plot is 96 blocks by 96 blocks. Make sure to stay within this area when building.
- Command Blocks vs Functions: It's recommended to use functions for better performance and version control. However, if you prefer command blocks, include the execute command (shown above) at the beginning of your command block chains for toggleable functionality.
- Scoring System: You're in charge of awarding points to players. There are two scoring options:
  - Podium: 1st place gets 3 points, 2nd place gets 2 points, and 3rd place gets 1 point.
  - Timed: All players who finish within the allocated time get 1 point.
- Building Considerations: Your plot borders another player's plot, so be mindful of shared blocks like water or lava.
- Adventure Mode: Players will be in adventure mode. If your minigame involves mining or placing blocks, use the /give command with "allow" or "deny" to control block interactions.
- Player Queries: You can query various properties of players using the provided list. Additionally, health can be detected through the "health" scoreboard.

Feel free to seek help from other players in the Bedrock Commands Community Discord if needed. Enjoy the Summer Collaborative Project!
