## Pokemon Crystal Any% Glitchless FAQ

### What's the goal of the speedrun?
- The goal is to beat all 8 Johto Gym Leaders, beat the Elite 4, beat all 8 Kanto Gym Leaders, then beat Red at Mt. Silver, without using arbitrary code execution (ACE), save corruption, or glitches.

### What's the tl;dr of the route?
- The start of the run is _very_ manip heavy. We manipulate a perfect (or near perfect) Toto to use to get past Whitney, then we main switch to an RNG manipulated Raikou with great stats and HP Ice. From there, we pretty much sweep the rest of the game.

### What's the current world record?
- The current world record is a [3:08:13](https://www.speedrun.com/pkmncrystal/runs/yw00623m) by WaveWarrior.

### Why do you keep resetting the game so much in the beginning?
- I'm setting up a specific RNG manipulation in order to make the game faster to beat. Specifically, I'm attempting to set my Trainer ID (TID) to match Kenya's OT. Doing this will prevent it from getting boosted exp during the Rival 3 fight and save one level up.

### Why do you wait ~50 seconds before starting a new game?
- The game has a hidden timer and we need to confirm our Day/Time in the new game setup at a specific point in that timer. If we don't do this properly, future manips will likely fail.

### What other RNG manips do you do?
1) TID manip. I attempt to manipulate my TID to also be `01001`. If I succeed, Kenya will have the same OT as my trainer id, so it will not gain boosted exp and save a level up (~3s). There's no penalty for missing TID.
2) Totodile manip, which allows us to get a Totodile with perfect or near perfect stats to get us through the early game
3) On Route 29. (2 times), to manipulate 0 encounters through the grass tiles
4) On Route 30. We manipulate 0 encounters through the grass tiles on the way to Violet City
5) On Route 32. We manipulate 0 encounters through the grass tiles and a spinner pass
6) Raikou manip. We manipulate a Raikou with extremely good stats and Hidden Power - Ice. This is our main carry through the game.
7) Douglas manip. There is a spinner inside Pryce's gym that we cannot dodge reliably, so we sometimes perform a final manipulation to get past him without fighting.

### What are spinners?
- Spinners are a classification of trainers that spin rapidly in place, making them difficult to avoid if we need to pass them.
- There are some strategies used to improve your chances of passing by them safely. This is why you'll see me pause in front of them; I'm trying to react quickly to them spinning a particular direction.
- Unless a spinner is stuck, you are never "guaranteed" to pass a spinner successfully, but good passes should be over 90% to not be seen.
- On this route, there are 31 spinner passes that are performed.

### Why does your title say `-masterball`?
- I have recently (around March 2025) developed a "yoloball" manip for Raikou, where I am able to catch it with a Poke Ball instead of a Master Ball.
- This removes the entire need to go to the Radio Tower and do the lottery, and removes the need for LID manip. If done successfully, it should save around 30-35s.

### Why does your title say `+guardspec`?
- I've recently started routing in the usage of a Guard Spec. when fighting Karen instead of buying and using an X Accuracy.
- The guard spec. Karen fight ends up being slightly slower than the X Acc Karen fight, but the X Acc route required me to sell all my Poke Balls in order to afford all my healing items + x accuracy.
- On runs where I am severely behind, I may forgo to use the guard spec. and fall back to the faster/riskier Karen strat of forcing your HP to be under 50% entering Karen, which strongly encourages Karen's AI to use Faint Attack instead of Sand Attack or Confuse Ray.

### What are the extended manips?
- For both of the Rt 29 Manip passes, I have designed "extended manips". For each pass, it means that on top of no encounters up the route, if I execute correctly I can continue the RNG manipulation for favorable outcomes.
- For the first pass, if I am able to clear all the textboxes in the Mr. Pokemon house perfectly, I can manipulate no encounters on the way down Rt 30. If I do this successfully and clear the Rival textboxes properly, I can manipulate a turn 1 Tackle instead of a growl.
  - Encounters are worth around 13.5 seconds, and a Growl from Rival 1 usually costs around 2 turns (~12 seconds).
  - This manip is particularly difficult and I am still attempting to build consistency.
- For the second pass, if I clear the textboxes for the Mikey fight perfectly and perfectly select the move Scratch, I can manipulate a crit that will one-hit KO his Pidgey, saving a turn.

### What is berry-ful?
- As of 2025 May 10, I have started doing run where you never unequip the berry from Totodile. This berry is primarily used to heal during the Spearow fight inside Falkner's gym.
- Normally, we unequip the berry at the start of Rt29, fight Rival 1 and Mikey, then reequip the berry. This is mainly because you are very likely to get below 50% fighting Rival 1, which will use up your berry.
- I have updated the extended manip to manipulate a Growl fail (or Tackle miss in rare cases) on turn 1. This means you are highly likely to win the fight without using the berry.
- This strategy saves around 8 seconds overall.

### What is that timer on the top of your LiveSplit layout?
- That is [FlowTimer](https://github.com/stringflow/flowtimer), a program that acts like a metronome in order to hit frame precise manipulations. Whenever that timer is ticking down, it means I'm preparing for a manipulation and I'm trying to time hitting A when the timer reaches 0.

### What's your goal time? Are you going for world record?
- 3:07:XX. With the development of Rt29 extended manips and Raikou yoloball, I believe this time is very achievable with a spinnerless run and first try Raikou.

### What are the major places you can save time in your PB?
- My PB has a very subpar early game (Bugsy/Whitney/Rival 3/Morty). I also lost around 20 seconds in the final Red split, and some not unsignificant timesave in Jasmine/Clair/Will/Misty/Surge.

### Why do you sometimes compare against juanly when his PB is slower than yours?
- Juanly is someone I've known the longest in PSR and it's fun to compare against his run. If the run ends up going to late game, I might switch to another comparison for a better idea of what my pace is.

### Why does your game audio get messed up every once in a while?
- There's a current bug with Windows and the OBS audio application capture. It's a [known issue](https://github.com/obsproject/obs-studio/issues/8064). Until this issue gets resolved, there isn't much I can do.
