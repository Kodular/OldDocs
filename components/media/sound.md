# Sound

A multimedia component that plays sound files and optionally vibrates for the number of milliseconds \(thousandths of a second\) specified in the Blocks Editor. The name of the sound file to play can be specified either in the Designer or in the Blocks Editor.

For supported sound file formats, see Android Supported Media Formats.

This Sound component is best for short sound files, such as sound effects, while the Player component is more efficient for longer sounds, such as songs.

## Properties

### MinimumInterval

The minimum interval, in milliseconds, between sounds. If you play a sound, all further Play\(\) calls will be ignored until the interval has elapsed.

### Source

The name of the sound file. Only certain formats are supported. See [http://developer.android.com/guide/appendix/media-formats.html](http://developer.android.com/guide/appendix/media-formats.html).

## Events

none

## Methods

### Pause\(\)

Pauses playing the sound if it is being played.

### Play\(\)

Plays the sound.

### Resume\(\)

Resumes playing the sound after a pause.

### Stop\(\)

Stops playing the sound if it is being played.

### Vibrate\(number millisecs\)

Vibrates for the specified number of milliseconds.

