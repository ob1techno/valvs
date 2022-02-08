# Vālvs
A cascading quad tube VCA module in Eurorack format, using NOS Soviet 1Ж24Б tubes; as used in the Спутник 1 satellite and Восток 1 spacecraft!

Vālvs provides four gnarly tube VCAs with adjustable, switchable distortion, feedback, drive and gain controls.

Vālvs’ outputs are daisy-chained, allowing adjacent groups of 2, 3, or all 4 channels to be mixed together.

Based on/inspired by the work of [Ken Stone](https://www.elby-designs.com/webtek/cgs/cgs65/cgs65_vca.html), [L-1](http://l-1.su/TubeVCA.html) and [Émilie Gillet](https://mutable-instruments.net/modules/veils/).

_N.B. this is currently in development and not verified as working_

## Notes

### Noise
This is inherently a pretty noisy circuit. The tubes can be a little microphonic (this can be improved a little by mounting with some foam/padding between tube and board). The LEDs in Ken Stone's original design injected some more noise as they were connected to the tube's cathode which is in the signal path. L-1's design removes the LEDs, replacing with a 1/2W resistor to ground. I've built the circuit both ways and L-1's design is definitely less noisy. I originally thought I preferred the sound with the LEDs, but with all four VCAs mixed, the noise is too noticable, so I've gone with a resistor to ground! I've kept the LEDs to light the tubes, but these are now powered separately, away from the signal path. Even so, these are still quite noisy VCAs, though I prefer the term characterful!

### Disclaimer
I am not an electronic engineer. I am a musician with a keen interest in synthesis and electronics. I am entirely self-taught and I'm sure I have made many mistakes. I have tried to ensure that this works well before publishing my work, but this is presented as-is and with no guarantees or acceptance of responsibility on my part. I'd welcome any feedback and I am interested in improving the design; please use the issues section. I also make no promises to support this project, but do get in touch and I'll help if I can.

---

### v1.01 panel design

![Prototype Panel](/Images/ValvsPanel.png)

---

### v1.01 PCB front 

![Prototype PCB Front](/Images/ValvsPcbFront.png)

N.B. - an incorrect 3D model has been used for the tubes here as I couldn't find the right one!

---

### v1.01 PCB rear

![Prototype PCB Rear](/Images/ValvsPcbRear.png)

---

### v0.7 prototype build

![Prototype v0.7 Build](/Images/Valvs07Front.png)

![Prototype v0.7 Build](/Images/Valvs07Rear.png)

---

### v0.3 prototype build

![Prototype v0.3 Build](/Images/Valvs03.png)

![Prototype v0.3 Build](/Images/Valvs03on.png)

