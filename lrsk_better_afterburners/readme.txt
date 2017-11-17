This is a small combat tweak that hopefully will make afterburners more worthwhile by giving them an evasion multiplier. Now your corvettes should reach the enemy faster AND stay alive longer in the dogfight!

---

I need to explain the function in a bit more math depth because the in-game tooltip might be deceptive. The way it's presented, it seems like it will add 10 or 20 to the evasion rate percentage, but that's not what it really does as it uses "ship_evasion_mult" (a multiplier) rather than "ship_evasion_add" (an added value). What's meant by a "multiplier" here is that it multiplies the evasion rate by a certain percentage. For basic afterburners, this is 110% and for advanced this is 120%. That's what the displayed +10% or +20% actually mean. In other words, they will multiply whatever evasion rate a ship has by 1.1 or 1.2.

Example: Base corvettes have an evasion of 60%. Basic afterburners increase this to 60% * 1.1 = 66% and advanced afterburners increase this to 60% * 1.2 = 72%. This is applied to evasion after other added values. In this example, if our corvette has ion thrusters ("+3 chance to evade"), giving it advanced afterburners will increase its evasion to (60% + 3%) * 1.2 = 75.6%.

I would welcome feedback about how this affects combat in the game. I'm somewhat pleased with the results but I don't want it to be OP and don't really have enough testing to tell whether this makes afterburners "too good." The new version reduced the value of the evasion multiplier both to reduce the effect and to make things work better with a companion mod that improves the Enigmatic Encoder and Decoder.

Compatibility note: This mod unavoidably replaces component_templates/00_utilities_afterburners.txt and will likely conflict with any other mod changing how afterburners work.