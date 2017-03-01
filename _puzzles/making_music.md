---
layout: page
title: Making Music
permalink: /puzzle/making-music
hide: false
term: "Winter 2016-17"
week: 7
solutions: week7_making_music
---

In previous weeks, we have worked with drawing graphics. Today, however, we are going to work to create sounds.

## The Challenge
Today's goal is to find a way to output sound so that your program can play a major scale. This might be done by playing pure frequencies or by using a library. Once you've found a way to create a major scale, explore other sounds you can create such as a minor scale (natural, harmonic, or melodic) or simple melodies like "Hot Cross Buns." From there, see if you can't find a way to play chords as well!

## Helpful Links
Python (Windows Only): [winsound](https://docs.python.org/3.6/library/winsound.html)

```
import winsound

frequency = 262	 # The frequency of c4 (middle C)
duration = 1000 # Note length in milliseconds

winsound.Beep(frequency, duration) # Plays c4 for 1 second
```

C++ (Windows): [beep](https://msdn.microsoft.com/en-us/library/windows/desktop/ms679277.aspx)

```
Beep(262, 1000); // Plays c4 for 1 second
```

Java: [JFugue](http://www.jfugue.org/index.html)

```
import org.jfugue.player.Player;

public class Main {
  public static void main(String[] args) {
    Player player = new Player();
    player.play("C"); // Plays a C note
  }
}
```

Python: [PyAudio](https://people.csail.mit.edu/hubert/pyaudio/)
(This is more complicated. The example was taken from [AskUbuntu](http://askubuntu.com/questions/202355/how-to-play-a-fixed-frequency-sound-using-python))

```
import math
import pyaudio

#sudo apt-get install python-pyaudio
PyAudio = pyaudio.PyAudio

#See http://en.wikipedia.org/wiki/Bit_rate#Audio
BITRATE = 16000 #number of frames per second/frameset.      

#See http://www.phy.mtu.edu/~suits/notefreqs.html
FREQUENCY = 261.63 #Hz, waves per second, 261.63=C4-note.
LENGTH = 1.2232 #seconds to play sound

NUMBEROFFRAMES = int(BITRATE * LENGTH)
RESTFRAMES = NUMBEROFFRAMES % BITRATE
WAVEDATA = ''    

for x in xrange(NUMBEROFFRAMES):
 WAVEDATA = WAVEDATA+chr(int(math.sin(x/((BITRATE/FREQUENCY)/math.pi))*127+128))    

#fill remainder of frameset with silence
for x in xrange(RESTFRAMES):
 WAVEDATA = WAVEDATA+chr(128)

p = PyAudio()
stream = p.open(format = p.get_format_from_width(1),
                channels = 1,
                rate = BITRATE,
                output = True)
stream.write(WAVEDATA)
stream.stop_stream()
stream.close()
p.terminate()
```


## Bonus Challenge 1
Find a way to encode the sound data your program creates into a WAV file.

## Bonus Challenge 2
Given a list of chords or notes, interpret and play those sounds:

```
C,G,A,F
```

is a familiar chord pattern to try to get your program to play.
