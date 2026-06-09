# ASCII Aquarium v2.20 Release Notes

_Changes since v1.67_

ASCII Aquarium has grown from a charming little text tank into a much more capable desktop aquarium. Same fishy soul, far more polish on the glass. There are now richer backgrounds, lighting controls, scheduled feeding, and a proper clock personality.

Short version: this is still the same little CYD fish tank, just with more polish, more life, and a lot more _fin-ish_.

## Headline Changes

### The Tank Got a Real Background System

v1.67 had a much simpler visual setup. v2.20 now has a full background system
with styles and selectable colours.

Current background styles:

- **Black**: the classic deep-water void.
- **Dithered**: a retro pixel-textured gradient with selectable colour.
- **Smooth**: a cleaner top fade with selectable colour.
- **Flowers**: subtle pixel flower shapes behind the aquarium.

The dithered and smooth gradients now use a higher-fidelity rendering path on the CYD, so the blues and other colours look smoother without turning the frame rate into fish food. The default first-install look is now the blue dithered fade. The dithered and smooth backgrounds now use the shared background colour picker, so blue, purple, sunset-ish, green, cyan, and other colours can all swim in the same current.

### LCD Backlight and RGB Ambient LED

A hidden **B** button now opens the Backlight panel.

Backlight and ambient controls include:

- LCD brightness.
- Ambient RGB LED on/off.
- Ambient brightness.
- Ambient colour mode.
- Ambient colour picker.
- Background-linked ambient colour.

The ambient LED can follow the selected background colour or use its own picked colour. This lets the tank glow with the display instead of simply sitting next to it like a confused status light.

### Light Schedule and Tap-to-Wake

The Backlight panel now has a **Schedule** dialog for controlling when the LCD
and/or ambient LED should be lit.

Light Schedule features:

- Global schedule on/off.
- Start hour.
- End hour.
- Dim time from `1m` to `1h`.
- Dimming target:
  - None
  - LCD only
  - Ambient LED only
  - Both

The default schedule is off, and default dimming mode is None.

When enabled, the schedule fades the selected lights up at the start of the day and fades them down at the end. For example, with an `8am` to `8pm` schedule and a `1h` dim time, the selected lights fade in from `7am` to `8am`, stay at the chosen brightness, then fade down from `7pm` to `8pm`.

If the display is dimmed or off after hours, tapping the screen wakes the scheduled lights to their configured brightness, then fades them back down over one minute. The fish may be asleep, but customer service remains available.

### Timed Events and Auto Feed

The Tank settings now include a **Timed Events** dialog. This keeps the aquarium's occasional events in one place:

- Octopus frequency
- Seahorse frequency
- Auto Feed frequency

Auto Feed was added for setups where tapping the touchscreen is inconvenient, especially beam-splitter cube builds. It can be off, or set to various frequencies.

When Auto Feed runs, it sprinkles multiple flakes across the top of the tank in a short left-to-right or right-to-left pass. This looks more natural than one pile of food appearing in a single spot, and it gives the fish a little buffet line to chase.

Default Auto Feed is off. The fish are enthusiastic, but we are not trying to run an all-you-can-eat reef.

### 20 Selectable ASCII clock fonts.

The large ASCII clock renders behind the fish, bubbles, seaweed, food, octopus, and seahorse, so it becomes part of the aquarium background rather than a UI label sitting on top of everything.

Included ASCII clock fonts:

Standard, Bulbhead, Doom, Graceful, Ogre, Small, Soft, 3D-ASCII, Chunky, Cricket, Fuzzy, Greek, Larry 3D, LCD, Lean, NT Greek, Puffy, Rammstein, Stop, and Swan.

The default is still **Standard**, because a clock font should earn its drama.
