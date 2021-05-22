# Responsive Web Audio Metronome

![alt tag](assets/img/screenshot.png)

## Online Demo of Javascript Offline Metronome
[Demo Javascript Metronome](https://niebert.github.io/metronome)

Issues after fork from Scott Hudsons metronome: 
* Icons for play button were missing - check remote CSS
* Chrome support for Webworkers to run offline - already mentioned by Scott Hudson 2016 - check causes

## Based on Offline Metronome of Scott Hudson
Scsing @cwilso's [HTML5 demo metronome](http://webaudiodemos.appspot.com/metronome/index.html) as a starting point, I added several features commonly seen in professional metronomes, including:

* variable meter input
* support for triplet subdivisions
* master volume toggling
* accent volume toggling
* subdivision volume toggling
* material design UI

Adding triplet note support was the trickiest, since it required converting the base note interval from a 16th note to a twelvelet, which contains both eighth note and sixteenth note intervals (thanks college drumline days).  The scheduler picks out the relevant subdivisions in the polyrhythm and mutes the rest. This worked way better than simultaneously scheduling duple subdivisions and triple subdivisions, especially with the variable tempo input.


### Setup
1. clone the repository
2. open `index.html` using a broswer other than Chrome (Chrome doesn't like running web workers locally apparently)

### Todos
* toggle note pitches
* tap tempo detection
* easy sound file import
* add visual metronome
