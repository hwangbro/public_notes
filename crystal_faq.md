## Pokemon Crystal Any% Glitchless FAQ

### What's the goal of the speedrun?
- The goal is to beat all 8 Johto Gym Leaders, beat the Elite 4, beat all 8 Kanto Gym Leaders, then beat Red at Mt. Silver, without using arbitrary code execution (ACE), save corruption, or glitches.

### What's the tl;dr of the route?
- The start of the run is _very_ manip heavy. We manipulate a perfect (or near perfect) Toto to use to get past Whitney, then we main switch to an RNG manipulated Raikou with great stats and HP Ice. From there, we pretty much sweep the rest of the game.

### What's the current world record?
- The current world record is a [3:07:26](https://youtu.be/FulIuHKR7oo) by me.

### Why do you keep resetting the game so much in the beginning?
- I'm setting up a specific RNG manipulation in order to make the game faster to beat. Specifically, I'm attempting to set my Trainer ID (TID) to match Kenya's OT. Doing this will prevent it from getting boosted exp during the Rival 3 fight and save one level up.

### Why do you wait ~50 seconds before starting a new game?
- The game has a hidden timer and we need to confirm our Day/Time in the new game setup at a specific point in that timer. If we don't do this properly, future manips will likely fail.

### What other RNG manips do you do?
1) TID manip. I attempt to manipulate my TID to also be `01001`. If I succeed, Kenya will have the same OT as my trainer id, so it will not gain boosted exp and save a level up (~3s). There's no penalty for missing TID.
2) Extended Totodile manip, which allows us to get a Totodile with perfect or near perfect stats to get us through the early game
   b) This manip continues into Route 29 to guarantee 0 encounters
   c) This manip continues into Route 30 to guarantee 0 encounters on the way down
   d) This manip continues into Rival 1 to guarantee a perfect 3 turn Rival battle.
   e) This manip continues into Route 29 pass #2 to guarantee 0 encounters
   f) This manip continues into Mikey to guarantee a perfect 4 turn battle.
   g) This manip continues into Route 30/Route 31 to guarantee 0 encounters.
3) On Route 32. We manipulate 0 encounters through the grass tiles and a spinner pass
4) Raikou manip. We manipulate a Raikou with extremely good stats and Hidden Power - Ice. This is our main carry through the game.
5) Douglas manip. There is a spinner inside Pryce's gym that we cannot dodge reliably, so we sometimes perform a final manipulation to get past him without fighting.

### What are spinners?
- Spinners are a classification of trainers that spin rapidly in place, making them difficult to avoid if we need to pass them.
- There are some strategies used to improve your chances of passing by them safely. This is why you'll see me pause in front of them; I'm trying to react quickly to them spinning a particular direction.
- Unless a spinner is stuck, you are never "guaranteed" to pass a spinner successfully, but good passes should be over 90% to not be seen.
- On this route, there are 31 spinner passes that are performed.

### Why does your title say `-masterball`?
- I have recently (around March 2025) developed a "yoloball" manip for Raikou, where I am able to catch it with a Poke Ball instead of a Master Ball.
- This removes the entire need to go to the Radio Tower and do the lottery, and removes the need for LID manip. If done successfully, it should save around 30-35s.

### What are the extended manips?
- I have started attempting [Totodile Extended Manip](crystal_extended.md) which I have designed. This manip starts with a save + quit in the lab before getting Totodile and ends when I enter Falkner's gym.
- These strats are extremely difficult and require clearing over 160 textboxes perfectly (~5 frame window per textbox). If a single textbox is missed, the manip will fail.
- These strats can save over a 90 seconds over the strategies used in the previous world record (3:08:13 by WaveWarrior) and over a minute on the current world record by me.

### What is that timer on the top of your LiveSplit layout?
- That is [FlowTimer](https://github.com/stringflow/flowtimer), a program that acts like a metronome in order to hit frame precise manipulations. Whenever that timer is ticking down, it means I'm preparing for a manipulation and I'm trying to time hitting A when the timer reaches 0.

### What's your goal time? Are you going for world record?
- 3:06 or 3:05. 3:06 was already very possible with the strats the current world record employed, but with the "new" Toto extended manip, it is very achievable. 3:05 is possible but quite unlikely to happen.

### What are the major places you can save time in your PB?
- My PB doesn't use the new Toto manip so I can save around 50s in Falkner. I also lose a lot of time during the Jasmine/Will/Karen splits. The Bugsy/Whitney/Rival 3 splits are also a bit below average.

### Why do you sometimes compare against juanly when his PB is slower than yours?
- Juanly is someone I've known the longest in PSR and it's fun to compare against his run. If the run ends up going to late game, I might switch to another comparison for a better idea of what my pace is.

### Why does your game audio get messed up every once in a while?
- There's a current bug with Windows and the OBS audio application capture. It's a [known issue](https://github.com/obsproject/obs-studio/issues/8064). Until this issue gets resolved, there isn't much I can do.
