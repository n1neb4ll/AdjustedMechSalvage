# AdjustedMechSalvage
AdjustedMechSalvage is a BattleTech mod (using ModTek) that changes the rules that mech parts get generated.

## Requirements
* install [BattleTechModLoader](https://github.com/Mpstark/BattleTechModLoader/releases) using the [instructions here](https://github.com/Mpstark/BattleTechModLoader)
* install [ModTek](https://github.com/Mpstark/ModTek/releases) using the [instructions here](https://github.com/Mpstark/ModTek)

## Features
- Your own mechs now get destroyed and leave behind salvage.
- Number of salvage is now based the number of parts you destroyed.
- You get DefaultMechPartMax(number needed to assemble a mech) - DefaultMechPartMax / 5 parts for each arm or leg the target lost.
- CT lost is 0 parts

## Example: 
DefaultMechPartMax is set to 5:
- 5 - 1(leftleg destroyed) - 1(Rightleg destroyed) = 3 parts

DefaultMechPartMax is set to 3 or 5:
- CT destroyed, rightleg destroyed = 1 parts
- CT destroyed destroyed = 1 parts
- CT destroyed, rightleg destroyed, leftarm destroyed = 1 parts

DefaultMechPartMax is set to 3:
- 3 - 0,6(rightarm destroyed) - 0,6(rightleg destroyed) = 1,8 rounded to 2 parts

## Download
Downloads can be found on [github](https://github.com/Morphyum/AdjustedMechSalvage/releases).
    
## Settings
- ownMechsForFree - bool - default false - Places the parts of the mechs you loose yourself directly into your inventory instead of making you salvage them.
- ejectRecoveryBonus - float - default 0 - Flat Bonus to your recovery chance if you punshed out.
- incapacitatedRecoveryBonus - float - default 0 - Flat Bonus to your recovery chance if pilot got incapacitated.

Example: RecoveryRate set to 0.5 -> Can rolls 0-1 0.6 -> eject bonus is 0.15 -> 0.5+0.15 = 0.65 -> 0.6 is smaller then 0.65 so mech is recovered
       
## Install and use
- After installing BTML and ModTek, put the AdjustedMechSalvage folder into the \BATTLETECH\Mods\ folder.
- Change any settings in mods\AdjustedMechSalvage\StreamingAssets\data\simGameConstants\simGameConstants.json and settings.json if you would like to.
- Start the game
