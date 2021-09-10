# wavtestWorks
Test playing WAV files. Works!

Hardware:
- Pico LiPo 16MB (similar to the Raspberry Pico, except it has 16MB onboard Flash)
- Adafruit MAX 98357A (mono amplifier and DAC for i2s sound)
- a 4 Ohms 3 Watts mono speaker

Wiring:
- The "minus" (3rd Pin right) of the Pico goes to GND of the Amplifier
- The "plus" (5th Pin right) of the Pico goes to "Vin" of the Amplifier
- The GPIO2 (4th Pin left) of the Pico goes to "DIN" of the Amplifier
- The GPIO3 (5th Pin left) of the Pico goes to "BCLK" of the Amplifier
- The GPIO4 (6th Pin left) of the Pico goes to "LRC" of the Amplifier
- The "GAIN" and the "GND" Pins, both on the Amplifier, are directly connected

Working output as expected:
- German words "eins", "zwo", "drei" (which means "one", "two", "three") are spoken from the speaker
- Three lines of text are printed (each line with the name and lenght of the sample)
