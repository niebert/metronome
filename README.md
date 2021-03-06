# Responsive Web Audio Metronome

![alt tag](assets/img/screenshot.png)

## Online Demo of Javascript Offline Metronome
[Demo Javascript Metronome](https://niebert.github.io/metronome)

Issues after fork from Scott Hudsons metronome:
* Icons for play button were missing - check remote CSS
* Chrome support for Webworkers to run offline - already mentioned by Scott Hudson 2016 - check causes

## Based on Offline Metronome of Scott Hudson
This metronome is based on Scott Hudson great work for an Offline Javascript Metronome, that runs in your browser without internet connection.

## Global Offline Metronome
The [global offline metronome](https://niebert.github.io/globalmetronome) was based on this metronome of Scott Hudson to be used in online rehearsal e.g. for a choir.

![alt tag](assets/img/screenshot_globalmetronome.png)

See also **[Online Demo of Global Metronome](https://niebert.github.io/globalmetronome)**.

### History
Scott Hudson used @cwilso's [HTML5 demo metronome](http://webaudiodemos.appspot.com/metronome/index.html) as a starting point.
* Repository was used for testing to identify challenges mentioned by Scott Hudson e.g. Chrome.

### Features
Scott added several features to @cwilso's [HTML5 demo metronome](http://webaudiodemos.appspot.com/metronome/index.html) which are commonly seen in professional metronomes, including:

* variable meter input
* support for triplet subdivisions
* master volume toggling
* accent volume toggling
* subdivision volume toggling
* material design UI

Furthermore Scott added triplet note support, which was the trickiest to implement, since it required converting the base note interval from a 16th note to a twelvelet, which contains both eighth note and sixteenth note intervals.

### Offline Use
Scott mentioned that Chrome doesn't like running web workers locally apparently. Chrome is widely used browser and the offline check in 2021 of the Scott's metronome did not work in Chrome now (Download Global Metronome instead and start `index.html`).

### Setup
1. clone the repository or [download ZIP](https://github.com/niebert/globalmetronome/archive/refs/heads/main.zip) 
2. open `index.html` using a browser other than Chrome (Chrome doesn't like running web workers locally apparently)

### ToDos
* toggle note pitches
* tap tempo detection
* easy sound file import
* [add visual metronome - DONE in Global Metronome](https://niebert.github.io/globalmetronome)
* fixing the Chrome problem for offline use
