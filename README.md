# touchy

I wanted a way to visualize musical intervals within chords, in a layout that's not biased to a particular key (like a a piano style keyboard is).

This
- allows varied layout. So far I've played with 
  - a few octaves of chromatic (see screenshot)
  - guitar and uke layout
  - isometric with thirds and fifths
- optionally mentions
  - note name (disabled in screenshot below)
  - Intervals to all touched notes
- colors by consonance (blue) or dissonance (red)
- reacts to multitouch
- reacts to MIDI input
- plays to MIDI

![Animated screenshot of playing a major triad](/screenshot.gif?raw=true)

This is code leveraging the [Kivy](https://kivy.org/) framework, because it's a very convenient way to quickly make this sort of experiment - the first functional version was under 100 lines.


# Requirements
- [Kivy](https://kivy.org/doc/stable/gettingstarted/installation.html)
- [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) (optional) is one way to route MIDI to a DAW


# TODO
- change button behaviour
   - right now reacts twice
   - figure out whether/why changing button text makes it so slow to respond to lots of touches at once (is it relayouting?)
- actually add the code here

- figure out other realtimeish issues
- think more about the consonance/dissonance coloring

- packaging so I can offer download rather than 'please install these things'
 

# CONSIDER
- make it react to sliding touch
   - as in, hit all buttons you pass, not just the one you land the touch on
   - consider strumming, pitch bends

- add on-screen config, e.g. swapping to other layouts, what to show on buttons, switching midi channel

- add file config (e.g. for what MIDI device name to prefer)

- think about other musical concents I want to explore with this
   - make it smart about chords?

