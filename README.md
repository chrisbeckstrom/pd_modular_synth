# A modular synthesizer built in Pure Data

I love modular synthesis. I love Pure Data. Why build yet another modular synth in PD? Because why not!

I built a physical, mostly-analog modular synthesizer (more here: <http://chrisbeckstrom.com/main/the-modular>) and use this software modular for more sound sources and to test out ideas before I build real-world circuits. 

# How to use this stuff

Each module exists as a PD abstraction. To use a module, create a new PD file and instantiate the abstraction. For instance, if you want to use the `adsr` module, make sure your PD is configured to use the `pd_modular_synth` as a folder for patches and create an object called `adsr`. That should do it!

_I'm not 100% sure how you tell your PD to use the folder.. will add more later once I better understand how that all works_

# The approach

check out `notes.md` for more info about the approach and philosophy. Basically the modular operates using "cv" (audio between -1 and 1).

# Caveats

I'm no PD expert! I'm sure I'm doing plenty of things in very strange ways. That said, overall this stuff works, and that's all I really want. If you know a better way to do something, let me know! Or better yet, contribute!

-Chris


