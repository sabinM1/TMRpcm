## Forked repository of TMRpcm

<mark>Not planned to merge with the original, this fork is only for my tests with the [Recording](https://github.com/sabinM1/TMRpcm/blob/master/examples/xtraFeatures/Recording/Recording.ino) example. Really, it's no longer a library, there are only files that I've modified or created.</mark>

---

#### Failed recordings in [/WAVs/Fails/](https://github.com/sabinM1/TMRpcm/tree/master/WAVs/Fails);
#### Succesful recordings in [/WAVs/Ok/](https://github.com/sabinM1/TMRpcm/tree/master/WAVs/Fails);
#### Noise sample in [/WAVs/Noise/](https://github.com/sabinM1/TMRpcm/tree/master/WAVs/Noise);

### Note:
1. The noise could totally be my fault for not fiddling enought with the microphone or another thing that I'm not aware of. The [audio samples provided by the original author](https://github.com/sabinM1/TMRpcm/tree/master/audio_samples) are much better, it is probably something on my end.
2. The failed attempt(s) with:
 - ```_5v``` at the end are recordings with the mic put on 5v not 3.3v like the rest of them. I didn't find them to be any better so I went with 3.3v for the rest of them;
 - ```_voiceoverffs``` at the end has some voice in the background;
3. I tried denoising an *ok* recording with Audacity but no good.
4. The TMRpcm library can be used <b>but is not limited to</b> recording with a mircophone. For me personally I've used the library in another project that plays audio files from an SD card. If you are interested in this project *(aham shameless self promotion)* be sure to check out [speaker-sd](https://github.com/sabinM1/speaker-sd) on GitHub.

### If you want to recreate this project:
#### You will need:
 - a micro SD card module and a micro SD card;
 - a microphone /w amplifier module;
 - (optional) a Piezo speaker;
 - access to a computer with the Arduino IDE, for the serial input;
 - to modify the TMRpcm library, as mentioned in the [Recording](https://github.com/sabinM1/TMRpcm/blob/master/examples/xtraFeatures/Recording/Recording.ino) example;

---

### Original README:

```
Arduino library for asynchronous playback of PCM/WAV files direct from SD card

Utilizes standard Arduino SD library, SD card and output device (Speaker, Headphones, Amplifier, etc)

Documentation is available on the Wiki: https://github.com/TMRh20/TMRpcm/wiki

Recent Updates
Many new features have recently been added, and are in development. See the wiki: https://github.com/TMRh20/TMRpcm/wiki/Advanced-Features

Features

    PCM/WAV playback direct from SD card
    Main formats: WAV files, 8-bit, 8-32khz Sample Rate, mono. See the wiki for other options.
    Asynchronous Playback: Allows code in main loop to run while audio playback occurs.
    Single timer operation: TIMER1 (Uno,Mega) or TIMER3,4 or 5 (Mega)
    Complimentary output or dual speakers
    2x Oversampling
    Supported devices: Arduino Uno, Nano, Mega, etc.
    More! See the wiki https://github.com/TMRh20/TMRpcm/wiki/Advanced-Features
```
