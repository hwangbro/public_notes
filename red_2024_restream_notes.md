# Notes for Restreaming 2024 Red Tournament

## Setting up Stage Ten WHIP URLs
- Visit https://app.stageten.tv/startup, create free account
- Click `Pro Studio` on the sidebar
<img src="images/stageten_homescreen.png">
- Click `Skip` on the next page
<img src="images/stageten_skip.png">
- The next steps will have to be repeated for each runner:
    - Click `Add or Invite Feeds` in the top left panel, then open the participant URL in another tab
    <img src="images/stageten_add_invite.png">
    - Fill out a name for the runner and click `Accept Invitation`. It will not be displayed anywhere
    <img src="images/stageten_accept_invite.png">
    - On the next page, click `WHIP Source`, then `Copy` on the `WHIP SERVER URL`.
    <img src="images/stageten_whip_source.png">
    <img src="images/stageten_whip_url.png">
        - You will provide this URL to one runner to use as their OBS WHIP server.
    - Once they have copied this server URL, ask them to click `Start Streaming` in OBS and their feed should appear in the `Pro Studio` tab in StageTen
    - Click on the hamburger context menu in their feed and click `Copy Solo Link`. This is a link you will feed into the restreaming OBS to use as a browser source for this runner.
    <img src="images/stageten_copy_solo_link.png">
    - Repeat these steps for each runner until you should have all 3 feeds added into OBS
