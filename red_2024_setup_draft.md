# Pokemon Red 2024 Runner Tech Setup Guide

## OBS Setup
- Download [portable OBS](https://drive.google.com/file/d/1e_pUcq5JcJkLql5j2EsNO7yng-aop39D/view?usp=sharing)
- Unzip the folder and run `RED RUNNER OBS LAUNCH.bat`
    - Contains uniform layouts to make our restream efforts easier
- Modify the `GAME FEED` source in OBS and set it to capture your game feed (Emulator/Capture Card)
- If you are running on GSE, please enable `Hide Status Bar` in settings.
- If you are on console, you may have to crop your feed to only capture gameplay and fit it within the BLUE area in the layout. 
- If you plan on watching the restream or having music playing, please make sure OBS is capturing **only** your game audio and not full desktop audio
- Modify the `RUNNER NAME` text and set it to whatever name you would like to display on stream
- Your OBS preview should look something like this when you are done

    - <details><summary>Example</summary>
        <img src="images/obs_runner_preview.png">
        </details>

- During the tech check before your race, the restreamer will provide you a URL to stream to. You will **not** be streaming to your normal twitch channel unless the restreamer is having issues with this current setup.
    - Go into Settings -> Stream, ensure Service is set to `WHIP`, and place the given URL in the `Server` box.
- Once you click start streaming, the restreamers should be able to capture your stream feed. They will communicate with you if anything needs to be modified.
- **Please local record your run in case you disconnect from the restreaming setup.**
    - You will need to change the recording path. Please test this before your race to make sure you are able to record without issues.

## Y No Restream??
- Due to the large number of participants this year and limited resources, there is a chance your race might not be restreamed.
- If this is the case, one of the organizers or restreamers will reach out to your race group and let you know in advanced.
- You will be asked to stream (& local record) your race to your normal twitch channel, using racetime.gg
    - Layout is flexible here, as long as it contains your game feed and **livesplit timer**
- You may still be asked to do some small run verification, like palette changes, before the race begins.

## LiveSplit Setup
- It is recommended you use the following split names in an effort to standardize names to make split comparisons easier.
```
Nidoran
Brock
Route 3
Mt. Moon
Bridge
Misty
Surge
Fly
Flute
Koga
Erika
Blaine
Sabrina
Giovanni
Lorelei
Bruno
Agatha
Lance
Champion
Hall of Fame
```

## Racetime.gg Setup
- If you haven't already, create an account on [racetime.gg](https://racetime.gg/)
- Before your race starts, the restreamers should create a new race on racetime.gg. We strongly recommend joining the race through the LiveSplit-racetime.gg plugin.
    - Open LiveSplit, click `racetime.gg Races`, and you should see a new race for Pokemon Red/Blue. If this is your first time doing this through LiveSplit, it may prompt you to login and/or authorize LiveSplit.
- If you joined through LiveSplit, your timer should automatically be set to -15s before the race begins. Once everybody in the room clicks "Ready", the countdown will begin.
- You should click "New Game" when the timer hits "0" and the race will begin


## Pre-Race Setup
- Please pay attention to the racetime.gg race window, especially before the race starts and in the first few minutes in the race.
    - It will be the main form of communication for the restreamer/commentator to reach you during the race.
- The commentators/restreamers should communicate with you to set an initial palette before the race begins. This is a countermeasure against runners using pre-recorded runs.
- They should specify this in the form of a direction + optional button, e.g. `LEFT+A` or `UP`. Make sure you set this palette and are using it when you begin the race.

## Post-Race Setup
- After you are finished with your race and if you would like to join the stream, please join the `#Tournament Waiting Room` channel and someone will pull you into the restream/commentary channel.
