## Animal Crossing JiggleWiggler

Automatically pushes buttons so that your Switch doesn't go to sleep when idling in Animal Crossing. Really handy for leaving your island open for friends so they can come and... like... I dunno. Do stuff? Fish? Steal your shit? Don't ask me, dude.

This is based off of [Bertrandom's Snowball Thrower](https://github.com/bertrandom/snowball-thrower) for BotW.

Their full writeup is [here](https://medium.com/@bertrandom/automating-zelda-3b37127e24c8).

No warranty is implied or assumed. I am not liable for missing bells, items, broken Switches, rabid Tom Nooks, or any other disaster associated with using this. User takes sole responsibility for their actions.

#### How to use

This repository has been tested using a UNO r3.

LUFA has been included as a git submodule, check it out with recursive.

You'll need to get your UNO into [DFU mode](https://www.arduino.cc/en/Hacking/DFUProgramming8U2) first. Follow that guide and then stop before it has you flash the new DFU. Instead, be a rebel. Open a terminal window in the `No-Sleep-Till-NookLand` directory, then run:
`make && sudo dfu-programmer atmega16u2 erase && sudo dfu-programmer atmega16u2 flash Joystick.hex`

And there's nothing the police can do about it.

Now, open your Home menu for the Switch, go to Controllers, then Change Grip. Plug in your Arudino. Wait a few seconds and you should see a pro controller pop up. Pair up your other controller as player 2, and get back in Animal Crossing. Your player 2 controller will unpair, and this is fine. You're not playing right now. Your Arduino is... and it's kinda bad. But that's ok.

When you're back and ready to play, unplug your Arduino. The Switch will automatically pull up the Change Grip Order screen. Pair up your controller again and go do things.

Have fun!

#### Thanks

Thanks to Shiny Quagsire for his [Splatoon post printer](https://github.com/shinyquagsire23/Switch-Fightstick) and progmem for his [original discovery](https://github.com/progmem/Switch-Fightstick).
