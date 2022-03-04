# Vālvs
A cascading quad tube VCA module in Eurorack format (3U/32hp).

Vālvs provides four gnarly tube VCAs with drive, gain, feedback, and adjustable, switchable distortion controls.

Vālvs’ outputs are daisy-chained, allowing adjacent groups of 2, 3, or all 4 channels to be mixed together.

![Vālvs v1.01 Front](/Images/Valvs101Front.png)
*"OG" unit*

![Vālvs v1.01 Stealth Mode](/Images/Valvs101FrontStealth.png)
*"Stealth" unit*

![Vālvs v1.01 Rear](/Images/Valvs101Rear.png)
*Rear view*

Based on/inspired by the work of [Ken Stone](https://www.elby-designs.com/webtek/cgs/cgs65/cgs65_vca.html), [L-1](http://l-1.su/TubeVCA.html) and [Émilie Gillet](https://mutable-instruments.net/modules/veils/), using NOS Soviet 1Ж24Б tubes; as used in the Спутник 1 satellite and Восток 1 spacecraft!

## Demos
#### Single channel audio demo
[![Vālvs - Quad Tube VCA - Single channel audio demo](https://yt-embed.herokuapp.com/embed?v=XpYaYiyOpng)](https://www.youtube.com/watch?v=XpYaYiyOpng "Vālvs - Quad Tube VCA - Single channel audio demo")

#### Mixer demo
[![Vālvs - Quad Tube VCA - Mixer demo](https://yt-embed.herokuapp.com/embed?v=zRkru6GmQA4)](https://www.youtube.com/watch?v=zRkru6GmQA4 "Vālvs - Quad Tube VCA - Mixer demo")

## [Build Guide](https://github.com/ob1techno/valvs/wiki/Vālvs-v1.01---Build-Guide) 
The [build guide](https://github.com/ob1techno/valvs/wiki/Vālvs-v1.01---Build-Guide) is available [in the wiki](https://github.com/ob1techno/valvs/wiki/Vālvs-v1.01---Build-Guide).

## Notes

### Calibration/Adjustment
There are no hard and fast rules here. The module is intended to be pretty flexible in terms of gain/distortion so it's very much a case of setting it up to your own taste. You could calibrate each of the 4 VCAs as closely as possible to each other to keep things consistent or you could set each up to have a different character/flavour. 

Each VCA has 4 trimmers on the back of the PCB:

- Plate; this adjusts the plate resistance between 8.2k and 28.2k, which affects the overall gain of the VCA
- CV Init; this adjusts the initial gain voltage, which can be trimmed to ensure the VCA closes completely
- Clean; adjusts the amount of distortion for the "Clean" mode
- Dist; adjusts the amount of distortion for the "Dirty" mode

It's _fairly_ important to get the CV Init trimmed correctly to avoid any audible bleed, but other than that, it's down to taste. You shoud be aware that with additional gain/distortion, there will be inevitable additional noise, so experiment to find the sweet spots.

### Noise
This is inherently a pretty noisy circuit. The tubes can be a little microphonic (this can be improved a little by mounting with some foam/padding between tube and board). The LEDs in Ken Stone's original design injected some more noise as they were connected to the tube's cathode which is in the signal path. L-1's design removes the LEDs, replacing with a 1/2W resistor to ground. 

I've built the circuit both ways and L-1's design is definitely less noisy. I originally thought I preferred the sound with the LEDs, but with all four VCAs mixed, the noise is too noticable, so I've gone with a resistor to ground! I've kept the LEDs to light the tubes, but these are now powered separately, away from the signal path. Even so, these are still quite noisy VCAs, though I prefer the term characterful!

### KiCad Components

I used some KiCad components/footprints that you might need to install if you want to edit the PCB files. You can find those here:
- [EuroCad](https://github.com/nebs/eurocad)
- [E-Switch](https://www.snapeda.com/parts/100SP1T1B4M2QE/E-Switch/view-part/)

### Parts/Construction
I selected parts for this module based on several factors; what I had in stock already, parts I am familiar with and like to use, availability, etc. This means it may not be the easiest module for some to build. For example, I've used 0603 passives, where I could probably have fit a larger size, or used through-hole components. I made this decision because I have a large stock of 0603 passives and I personally prefer SMT to THT. That said, I don't think this is a difficult build. I've built a few of them and it's a relatively low part count per VCA, so quite quick to put together. The surface mount components used should make this suitable for SMD fabrication/assembly services, though so far I've only built them by hand.

The construction should all be self explanatory as it's just a single board. Parts go on the side where their silkscreen is (although if you used particularly tall film box caps, you might need to move them to the back). 

There's also the option of mounting the trimmers for the clean/dirty distortion on the front of the PCB and drilling holes so they're adjustable from the front, if you like that sort of thing. 

It's worth using some heatshrink on the tube legs for peace of mind, though not strictly necessary, and I like to use some acetate sheet to fill the windows in case of dust, stray cables, etc.

[There are some build photos in the wiki.](https://github.com/ob1techno/valvs/wiki/Vālvs-v1.01---Build-Guide)

### Disclaimer
I am not an electronic engineer. I am a musician/programmer with a keen interest in synthesis and electronics. I am entirely self-taught; this was my first project using KiCad and I'm sure I have made many mistakes. 

I have tried to ensure that this works well before publishing my work, but this is presented as-is and with no guarantees or acceptance of responsibility on my part. I'd welcome any feedback and I am interested in improving the design; please use the issues section or submit a pull request. 

I also make no promises to support this project, but do get in touch and I'll help if I can. 

