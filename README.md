# dual screen sbc handheld

## project idea

i want to build a clamshell handheld around an sbc, kind of like a 3ds but bigger. the goal is to play pokemon, zelda, and other ds/3ds games, plus older systems.

the project will use a custom 3d-printed case first, then maybe a cnc-milled chassis once the layout is proven. i want the screens, controls, cooling, and battery to fit inside the handheld instead of just putting a mini pc in a case.

## main parts

- **computer:** orange pi 5, 8gb
- **top screen:** 7-inch hdmi display
- **bottom screen:** 5-inch hdmi touchscreen
- **video connections:** top screen to the orange pi's hdmi port; bottom screen through a usb-c displayport-to-hdmi adapter
- **controls:** d-pad, abxy buttons, l/r buttons, start/select, and at least one analog stick
- **controls board:** a usb gamepad board or a small microcontroller that acts like a usb gamepad
- **cooling:** heatsink and fan for the orange pi
- **storage:** microsd card for the operating system and emulator
- **audio:** small speakers, with a headphone option if it fits
- **case:** 3d-printed prototype with a hinge; cnc version comes later
- **power:** wall power for the first tests; portable battery system after the rest works

## screen setup

the two screens don’t need to be the same size. the 7-inch screen will show the top game screen, and the 5-inch touchscreen will show the bottom one.

i want to keep the game image at the right shape instead of stretching it to fill the display. if the screen and game screen have different aspect ratios, the emulator can leave blank space around the picture.

the orange pi 5 has one hdmi port and displayport over usb-c, so the two hdmi displays need different connections. the operating system and emulator still need to recognize both displays and put the game screens on the right ones.

## roadmap

### 1. confirm the parts

- pick the exact 7-inch hdmi screen
- pick the exact 5-inch hdmi touchscreen
- make sure both screens include their display driver boards
- check how each screen is powered
- get a usb-c displayport-to-hdmi adapter for the second screen
- check the board, screens, cables, controls, and fan dimensions

**done when:** there’s a parts list with confirmed screen sizes, connectors, power needs, and measurements.

### 2. test the orange pi and screens on a desk

- boot the orange pi with a temporary operating system
- connect one screen to hdmi
- connect the other through usb-c displayport
- check whether both screens work at the same time
- try extending the desktop across both screens
- check whether the touchscreen works

**done when:** both screens show a picture at the same time and the bottom touchscreen registers input.

### 3. test games and screen layout

- install an emulator that supports the games i want to play
- try a few pokemon and zelda games i own
- set the top game screen to the 7-inch display
- set the bottom game screen to the 5-inch display
- check the picture shape, screen size, controls, and performance
- write down any settings that need to change for individual games

**done when:** the games i care about are playable and the two screens show the right parts of the game.

### 4. make a rough physical mockup

- make a cardboard or simple 3d-printed mockup
- leave openings for both screens
- put the controls where my hands can reach them
- check the hinge, viewing angle, and overall size
- leave room for the orange pi, fan, display boards, wires, and battery

**done when:** the open handheld feels okay to hold and the closed case has room for everything.

### 5. build the controls and prototype case

- connect the buttons and sticks to the controller board
- map the controls in the operating system and emulator
- print the first full case
- mount the screens and orange pi
- test cooling, cables, hinge movement, and screen alignment

**done when:** the handheld works as one wired prototype and can be opened and closed without pulling on the cables.

### 6. add portable power

- estimate how much power the board and both screens need
- choose a battery and power system that can provide stable power to the orange pi
- add charging, battery protection, and an accessible power switch
- test battery life and temperature during gameplay

**done when:** it runs safely from its battery for a useful amount of time.

### 7. make the finished chassis

- update the cad model using measurements from the working prototype
- make sure the cnc parts leave room for cooling and wiring
- check that the metal chassis doesn’t block wireless signals
- machine the chassis only after the layout and electronics are working

**done when:** the parts fit, the case closes properly, and the handheld survives normal use.
