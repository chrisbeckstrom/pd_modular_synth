## Pure Data Modular Synth ##

brainstorming, approach, etc.

### Key approach/philosophy ###
* Simple modules, low feature count per module
* Each module can be big or small. No need to be a slave to physical sizes like physical synths


### Specifics ###
* "CV" is audio signal between -1 and 1
* CV is converted to MIDI numbers (1-127) inside oscillators
* To use MIDI, it must first be converted to "CV" (_midi2cv_)
* Each module is an abstraction that lives in the main folder
* To add a module, just add it like any other PD object

### Modules ###
* VCO - simple oscillator, basic waves, LFO range to high (full range)
* VCA - simple VCA
* midi2cv - listens to _midiin_ and spits out CV and gate signals
* scope3 - a basic oscilloscope. _can only have one due to tabwrite needing to point to a specific array_
* comparator - compares two signals, HIGH when they match, LOW when they don't
* cubic-soft-clip
* more....