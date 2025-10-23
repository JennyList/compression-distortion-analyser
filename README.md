# A Distortion Analyser To Evaluate Audio Compression Algorithms
![The analyser as seen in GNU Radio Companion](ratio-mp3-distortion-rms.jpg)

Using a lossy compression algorithm such as MP3 introduces a level of distortion into the audio. This GNU Radio Project is an attempt to measure that distortion.

It works by taking two WAV files of the same sample, one of which has never been compressed, and the other of which has been compressed and then decoded back to WAV. It calculates the RMS of their difference, and compares it with the RMS of the never-compressed version to derive a ratio. If you need  percentage instead of a ratio, multiply the output figure by 100.

You can test it by comparing an input file with itself and getting a 0% figure, and by comparing it with noise and getting a high figure.

## Licence

This software is licensed under the [Creative Commons Attribution Share Alike 4.0 International licence](license.md).

The repository also contains two audio files derived from [Bongo_sound.wav](https://commons.wikimedia.org/wiki/File:Bongo_sound.wav), which is from MarleneAyni on Wikimedia Commons, and has a CC0 licence.
