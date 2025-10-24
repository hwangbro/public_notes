# Pokemon Red 2025 Tournament Tech Setup (In Progress)

## OBS Scene Setup
Download the [OBS setup](https://github.com/hwangbro/RedTournament/releases/download/v1/RED25_RUNNER_OBS.zip) for this year's tournament.

This is the OBS that you will be using to stream/record all of your tournament races this year. You can launch this OBS with the `RED RUNNER OBS LAUNCH.bat`.

### Runner Name
Click the `Runner Name` source and type in your own username. This will not be shown on stream, this is mainly to help identify your stream feeds from others for the restreamer's benefit.

### Game Feed
Click the `Game Feed` source and replace it with your own game feed. The game feed should cover as much of the blue area as possible.

If you are running on GSE, please enable `Hide Status Bar` in settings. There is also a filter on created for the `Game Feed` source to crop out the top menu bar for your convenience.

### Livesplit

#### Main Timer
There are two parts of LiveSplit that will be added to the layout. Click the `Livesplit Main Timer` source and point it to Livesplit. Crop out just your main timer into the `LIVESPLIT MAIN TIMER` area.

It does not need to fill the entire space, just make sure it does not leave the marked area.

This will not be shown on stream, this is to help the restreamers sync the different feeds during the race.

#### Clock
Inside the downloaded .zip file, there is a `LiveSplit.Clock.dll`. Copy this file into your Livesplit folder's `Components` directory.

When you open Livesplit, click `Edit Layout` and add the Clock component, under `Other`.

Double click the new component and remove anything inside `Text`. You can set or ignore the timezone, it doesn't matter too much. At the end, your settings should look something like this.

- <details><summary>Clock</summary>
    <img src="images/livesplit_clock_settings.png">
  <details>

Your Livesplit should now have a new row that displays the current date and time. In OBS, click the `Livesplit Clock`, source and point it to Livesplit. Crop out just the clock line into the `LIVESPLIT CLOCK` area.

It does not need to fill the entire space, just make sure it does not leave the marked area.

This will not be shown on stream, this is to help the restreamers sync the different feeds.

### Game Audio
If you are on emulator, double click the `Game Audio` source and point it to your emulator. You should see game audio reflected in the Audio Mixer.

If you are on console, you can remove this source, and I trust you will know how to get game audio into OBS depending on your setup.

Make sure that game audio is the **only** thing that is in the audio mixer; no desktop or mic sources.

### Example
After everything has been setup, please click the eyeball next to the `HIDE THIS WHEN FINISHED` group. This will remove all the two text labels for Livesplit.

Your layout should look something like this.

- <details><summary>Example</summary>
    <img src="images/obs_preview_example.png">
  </details>


At least 24 hours before your first tournament race, all runners must get their setup checked by one of the organizers or restream volunteers to ensure that everything is working properly.
