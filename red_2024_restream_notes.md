# Notes for Restreaming 2024 Red Tournament

## Pre Race

### Setting up Stage Ten WHIP URLs
- Visit https://app.stageten.tv/startup, create free account
- Click `Pro Studio` on the sidebar
        <details><summary>Example</summary>
        <img src="images/stageten_homescreen.png">    
        </details>

- Click `Skip` on the next page
        <details><summary>Example</summary>
        <img src="images/stageten_skip.png">
        </details>
- The next steps will have to be repeated for each runner:
    - Click `Add or Invite Feeds` in the top left panel, then open the participant URL in another tab
            <details><summary>Example</summary>
            <img src="images/stageten_add_invite.png">
            </details>
    - Fill out a name for the runner and click `Accept Invitation`. It will not be displayed anywhere
            <details><summary>Example</summary>
            <img src="images/stageten_accept_invite.png">
            </details>
    - On the next page, click `WHIP Source`, then `Copy` on the `WHIP SERVER URL`.
            <details><summary>Example</summary>
            <img src="images/stageten_whip_source.png">
            <img src="images/stageten_whip_url.png">
            </details>    
        - You will provide this URL to one runner to use as their OBS WHIP server.
    - Once they have copied this server URL, ask them to click `Start Streaming` in OBS and their feed should appear in the `Pro Studio` tab in StageTen
    - Click on the hamburger context menu in their feed and click `Copy Solo Link`. This is a link you will feed into the restreaming OBS to use as a browser source for this runner.
            <details><summary>Example</summary>
            <img src="images/stageten_copy_solo_link.png">
            </details>
    - Repeat these steps for each runner until you should have all 3 feeds added into OBS
    - If you are using the restream PC, please generate the broadcast and links on your own system to avoid overworking the PC
 
### Setting up racetime.gg room
- Create a new room in racetime.gg, join it yourself (as an organizers)
- Communicate with the runners, either via room or voice chat what the palette should be
- When all 3 runners are ready, quit the racetime.gg room in order to start the race
- Make sure to keep the racetime.gg chat room open in case you need to communicate with the runners.

### Setting up nodecg app

### Setting up OBS

### Setting up Commentator Feed in Discord

## During Race

### Switch audio feeds

### Switch scenes if necessary

### Stop timer on nodecg

## Post Race
- Mute all runner feeds
- Drag runners into commentator VC if they are unable to join themselves
- End stream once everyone is closing out
