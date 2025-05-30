# Raikou Yoloball Manip

## Goal
This manip uses the existing [Raikou Manip](https://pastebin.com/kHsktuhT), but catches it with a Poke Ball instead of a Master Ball.

## IGT Info
This manip aims for a 7 frame window between 8-14 which is guaranteed to work on all Raikous, but different Raikou frames can work on more frames outside this window.

| Frame | Failure IGTs |
| ----  | ------------ |
| 11    | 1-2, 15, 18, 30, 34, 37, 39, 41-57 |
| 12    | 6-7, 19-35, 42, 55 |
| 13    | 4, 20-36, 39, 41, 43, 51, 55 |

If you are "aiming" for F12/13 Raikou for better ranges, you can adjust the timer to aim for F8-18.

## FlowTimer Offsets
Target Frame: 12, Offset: 370

These offsets account for the following menus:
- Phone call to Mom before Rt 30 3/4 Manip
- One potion menu inside Falkner's Gym
- Menu to equip Bitter Berry and use Repel inside Union Cave
- One heal + menu inside Slowpoke Well. If you menu once in Slowpoke Well and use a potion and antidote, you would only add one `Heal`
- If you do not have to menu/heal inside Slowpoke Well, you would subtract one `Heal` and one `Menu`
- One menu + repel usage for the first Ilex Forest menu
- Teaching Cut and using Cut inside Ilex Forest
- One menu for 2nd repel in Ilex Forest
- Cutting the grass before Sudowoodo
- One menu to heal + repel after beating Whitney
- One menu to repel inside Burned Tower
- One menu (but not heals) to escape rope out of Burned Tower. If you need to use any healing items (potion/antidotes), they will need to be tracked.

The following will need to be tracked and manually added
- Any encounters/spinners
- Any accidentaly bag opens/healing items clicked
- Any antidote uses (and extra menus if they are not accounted for) including ones used in battle
- Any Paralyze heal uses
- Any extra healing menus not mentioned above, including healing before Whitney


The offset I use for the actual manip and yoloball is: `12169/38200`
This is 12169 for the A input to enter the game, and 38200 for the timed ball throw sequence for F12/13. These are merely starting points and will need to be calibrated.

## Misc
There are two different yoloball executions depending on which Raikou frame you hit.
If you hit Frame 11, the yoloball is a Pocket switch Right into a near immediate `A -> SELECT -> A`. This does not use an additional FlowTimer offset for timing the ball throw.
If you hit Frame 12 or Frame 13, the yoloball is 3x Pocket switch Left into a timed `A -> B -> A -> SELECT -> A`.

