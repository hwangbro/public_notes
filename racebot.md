# RacebotXD Documentation

## Functionality

- After all the racers in a watched race have finished a split, a message will be sent to all the racers' twitch channels for the current standings in the race.
- For you to receive updates in twitch, you'll have to connect your twitch account to SRL/RT.GG.
- After a race is finished, the results of the race are automatically formatted and posted in Discord
- This bot functions by posting to twitch chat. If you have your chat in follower only mode, feel free to ping me @hwangbro in discord and I can have the bot manually follow you.
- _(Experimental)_ Individual split times are being recorded by the bot and can be used to display interesting metrics about your race/pace/split segments over time.

## Discord Commands

### Watch
- `!watch <user>` to start watching a race, where <user> is either a twitch or rt.gg/srl name.
  - e.g. `!watch maddiict` if maddiict is in an active race room
- `!watch <race_id>` is also valid, where <race_id> is the rt.gg race "slug"
  - e.g. `!watch virtual-weedle-3498`
- There are extra "flags" that can be used add the end of `!watch` to modify how the bot behaves
  - `silent` or `silence`
    - e.g. `!watch maddiict silent` or `!watch virtual-weedle-3498 silence`
    - This allows the bot to track the race without posting split times to the runners twitch chat. The final result will still be posted in discord.
  - `spoiler`
    - e.g. `!watch <user> spoiler`
    - This makes the bot post the final result with spoiler tags, which can be useful for tournament races.
 
### Ignore
The bot will wait for all racers to finish a split beore announcing any splits. If someone is not connected through LiveSplit, or their websocket connection is broken, this bot will be waiting for splits that are never coming and will never announce.

There are two commands to tell Racebot to "ignore" a user and pretend their splits don't exist so it will announce without them.
- `!ignore <race_id> <user>`
  - This is used when a user should be ignored for this race only
  - e.g. `!ignore virtual-weedle-3498 slayerlol99`
- `!ignore_uesr <user>`
  - This is used when a user consistently has issues joining with LiveSplit and cannot be detected
  - e.g. `!ignore_user slayerlol99`
- `!unignore <race_id> <user>`
  - Reverses the effect of `!ignore` and tells the bot to try to track the user again.
-  `!unignore_user <user>`
  - Takes the user off of the persistent ignore list.
- `!ignored_users`
  - Lists everyone on the current persistent ignore list.

### Finish
In cases where a racer has finished but disconnected from the race client, their finish time can be recorded manually.
- `!finish_race <race_id> <user> <time>`, where <time> is formatted as `HH:MM:SS.MS`
  - e.g. `!finish_race calm-yolo-6223 hwangbroxd 02:06:31.38`

### Add Twitch Watchers
If you want updates to a race in a twitch channel that is not affiliated with a runner, you can use this command to do so.

This can be useful for spectating a tournament race, or restreams in general.

- `!add_watcher <race_id> <twitch_name>`
  - e.g. `!add_watcher virtual-weedle-3498 redracetv` will post updates to `virtual-weedle-3498` into the chat of `twitch.tv/redracetv`
  
### Update Comments
The bot will post the results of the race along with race comments after a race is finished.

If a comment is posted too late and was not picked up, you can use this commmand to ask the bot to refresh the results post with the current comments.

- `!update_comments <race_id>`
  - e.g. `!update_comments virtual-weedle-3498`
  - This will only work if a race is "finished", meaning the bot has posted the results in discord.

### Spoiler/Silence
Separate way to mark a race as "silent" or "spoiler"

- `!silence_race <race_id>`
- `!spoiler <race_id>`

### Racebot Info
Command that links to this documentation.

- `!racebot_info`

### Blacklist
If you think the race updates are too spammy and would prefer to not see them, you can add yourself to the blacklist to have the bot skip you when announcing splits.

- `!blacklist <user>`
  - e.g. `!blacklist slayerlol99`
- `!unblacklist <user>`
  - e.g. `!unblacklist slayerlol99`
- Note: the user here needs to be the twitch username

### Splits
If a race was recorded by the racebot, you can access the split data and view segment/split times. 

This command will post formatted splits for the given race.

- `!splits <race_id> <user>`
  - e.g. `!splits virtual-weedle-3498 maddiict`
  - The user here can be either the race client name (srl/rtgg) or twitch name.


## Twitch Commands
These are commands that can be run in a runner's twitch chat (or external watcher if added) and the bot will reply in that twitch chat.

### Standings
This command is used to get the most recent split for every racer and order them.

- `!standings`

### Watchlist
Normally the bot only posts updates when all entrants in a race finish a split. The `watch` command can be used to create a subset list of runners to receive personal updates for.

Split updates will only happen when the last user finishes a split. If they are very far behind other runners, this can lead to long delays between updates.

In these situations (or whenever you want), you can use this command to create a subset of racers to watch and receive updates for.

- `!watch <user1>, <user2>...`
  - e.g. `!watch hwangborxd, arayalol, franchewbacca`
    - In this example, I will receive a race update with only the 3 racers in my subset when we finish a split, and then later on I will receive the normal regular update when all the racers finish a split.
  - e.g. `!watch grogir`
    - In this example, I will get an update in chat with only `grogir`'s splits immediately when he splits, and then later on I will receive the normal regular update when all racers split.
  - Note that you are not automatically added to your own watchlit, but you can list yourself.
- `!watchlist`
  - This command will display your current watchlist.
- `!reset_watchlist`
  - This command will erase your current watchlist.

### Runner Info
Used to display all the entrants in the race and their twitch links.

- `!info`

### Multitwitch
Used to create a multitwitch link with all the runners.

- `!multitwitch`
