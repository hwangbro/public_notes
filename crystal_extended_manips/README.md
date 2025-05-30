# Pokemon Crystal Advanced/Extended Manips

## General Notes
These documents assume you know the basics of starting and setting up an IGT timer from how you would do it in Pokemon RBY. I recommend watching [this](https://www.youtube.com/watch?v=-jBTId8GuhI) tutorial from KinkMyBoot.

The main difference for IGT tracking between Gen 2 and Gen 1 is that you cannot restart your game on the same input as hitting `A` to save.

The way I chose to get around this is to time my hard reset on the same IGT tracking beep as the save. This means you should be hard resetting on the same IGT frame as hitting `A` to save.

For the first save, I wait 3 IGT seconds after hitting `A` to hard reset. For all other saves, I wait 2 IGT seconds.

## Calibration
All offsets given in manip documents were calibrated using GSE and should be used as a starting point. You can either use the Crystal Practice ROM to check IGT after a save, or use a program to get the IGT data from your .sav file.

I also used the following values in my `igtdelayers.json` for FlowTimer. Each manip page will tell you what in-game actions were accounted for, but you will need to account for variable events.
```
{
    "Game": "Crystal",
    "Delayers": [
        {
            "Name": "1f lag",
            "Delay": 1
        },
        {
            "Name": "Encounter",
            "Delay": 15.85
        },
        {
            "Name": "Heal",
            "Delay": 2
        },
        {
            "Name": "Menu",
            "Delay": 13
        },
    ]
}
```
Encounter is self explanatory and also used for any spinners hit.
Heal refers to the use of any item that takes you from your Item Pocket to Pokemon Menu. Any potion or status healing item fall in this category.
Menu refers to any additional time you load into the overworld from a start menu. Examples being opening and closing your Bag, Pokemon menu, Poke Gear, etc.

For example, if you are doing an unaccounted for menu that requires you to potion and antidote, you would add 1 `Menu` and 2 `Heal`

Start Flashes to pass spinner that do not open your pokemon/bag do not delay IGT

## Toto Manip
- Target frame: 5, Offset: 240
- Toto manip works from frame 0-7, but I aim for the 4-7 window for the slightly better FFEF 2nd Toto
- You should be hitting IGT second = 14 if you are planning on doing Rt 29 extended manip

## Rt30 3/4 Manip
- Target frame: 0, Offset: 220
- This manip works on all 60 IGT frames, but needs to be tracked in order for future manip tracking to work.
- This offset already assumes the phone call to Mom, but assumes you did not unequip and requip the berry.

## Manips
- [Route 29 -> Rival 1 Turn 1](rt29.md)
- [Route 29 -> Mikey Crit](mikey.md)
- [Route 32 -> Bill](rt32.md)
- [Raikou Yoloball](raikou.md)
