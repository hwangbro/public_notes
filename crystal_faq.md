## Pokemon Crystal Any% Glitchless FAQ

### What's the goal of the speedrun?
- The goal is to beat all 8 Johto Gym Leaders, beat the Elite 4, beat all 8 Kanto Gym Leaders, then beat Red at Mt. Silver, without using arbitrary code execution (ACE), save corruption, or glitches.

### What's the tl;dr of the route?
- The start of the run is _very_ manip heavy. We manipulate a perfect (or near perfect) Toto to use to get past Whitney, then we main switch to an RNG manipulated Raikou with great stats and HP Ice. From there, we pretty much sweep the rest of the game.

### What's the current world record?
- The current world record is a [3:08:13](https://www.speedrun.com/pkmncrystal/runs/yw00623m) by WaveWarrior.

### Why do you keep resetting the game so much in the beginning?
- I'm setting up a few RNG manipulations in order to make the game faster to beat.
  - One of the first things I'm doing is manipulating my Lucky ID (LID) to be 01001. This means that the lottery in Goldenrod will be using this number to determine matches and prizes.
  - 01001 is also the trainer ID of Kenya, a gift pokemon we pick up. So by manipulating our LID to be 01001, it ensures that Kenya will be a perfect match for us, giving us a master ball.

### Why do you wait ~50 seconds before starting a new game after LID manip?
- The game has a hidden timer and we need to confirm our Day/Time in the new game setup at a specific point in that timer. If we don't do this properly, future manips will likely fail.

### What other RNG manips do you do?
1) LID manip (described above)
2) TID manip. I attempt to manipulate my TID to also be `01001`. If I succeed, Kenya will have the same OT as my trainer id, so it will not gain boosted exp and save a level up (~3s). There's no penalty for missing TID.
3) Totodile manip, which allows us to get a Totodile with perfect or near perfect stats to get us through the early game
4) On Route 29. (2 times), to manipulate 0 encounters through the grass tiles
5) On Route 30. We manipulate 0 encounters through the grass tiles on the way to Violet City
6) On Route 32. We manipulate 0 encounters through the grass tiles and a spinner pass
7) Raikou manip. We manipulate a Raikou with extremely good stats and Hidden Power - Ice. This is our main carry through the game.
8) Douglas manip. There is a spinner inside Pryce's gym that we cannot dodge reliably, so we sometimes perform a final manipulation to get past him without fighting.

### What are spinners?
- Spinners are a classification of trainers that spin rapidly in place, making them difficult to avoid if we need to pass them.
- There are some strategies used to improve your chances of passing by them safely. This is why you'll see me pause in front of them; I'm trying to react quickly to them spinning a particular direction.
- On this route, there are 31 spinner passes that are performed.

### What is that timer on the top of your LiveSplit layout?
- That is [FlowTimer](https://github.com/stringflow/flowtimer), a program that acts like a metronome in order to hit frame precise manipulations. Whenever that timer is ticking down, it means I'm preparing for a manipulation and I'm trying to time hitting A when the timer reaches 0.

### What is step count and why does it matter?
- Raikou manip requires a very specific step count in order to work.
- This is based off of perfect movement all the way until Raikou, so any deviations or mistakes in movement have to be tracked.
- By the time I reach Burned Tower in Ecruteak, I'll have to make sure my step count is at an acceptable value, otherwise Raikou manip won't work.

### What's your goal time? Are you going for world record?
- I don't have a solid goal. Right now I'm aiming for around 3:09. Once I achieve that goal, I'll decide if I want to pursue a faster time. At this time, I'm **not** pursuing a world record time.

### Why do you compare against juanly when his PB is slower than yours?
- Juanly is someone I've known the longest in PSR and it's fun to compare against his run. If the run ends up going to late game, I might switch to another comparison for a better idea of what my pace is.

### Why does your game audio get messed up every once in a while?
- There's a current bug with Windows and the OBS audio application capture. It's a [known issue](https://github.com/obsproject/obs-studio/issues/8064) and the fix is supposedly in the next Windows 11 update, which I may or may not upgrade to. Until then, there isn't much I can do.
