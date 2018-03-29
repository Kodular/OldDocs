# Player

Multimedia component that plays audio and controls phone vibration. The name of a multimedia field is specified in the Source property, which can be set in the Designer or in the Blocks Editor. The length of time for a vibration is specified in the Blocks Editor in milliseconds \(thousandths of a second\).

For supported audio formats, see Android Supported Media Formats.

This component is best for long sound files, such as songs, while the Sound component is more efficient for short files, such as sound effects.

## Properties

### IsPlaying

Reports whether the media is playing

### Loop

If true, the player will loop when it plays. Setting Loop while the player is playing will affect the current playing.

### PlayOnlyInForeground

If true, the player will pause playing when leaving the current screen; if false \(default option\), the player continues playing whenever the current screen is displaying or not.

### Source

### Volume

Sets the volume to a number between 0 and 100

## Events

### Completed\(\)

Indicates that the media has reached the end

### OtherPlayerStarted\(\)

This event is signaled when another player has started \(and the current player is playing or paused, but not stopped\).

## Methods

### Pause\(\)

Suspends playing the media if it is playing.

### Start\(\)

Plays the media. If it was previously paused, the playing is resumed. If it was previously stopped, it starts from the beginning.

### Stop\(\)

Stops playing the media and seeks to the beginning of the song.

### Vibrate\(number milliseconds\)

Vibrates for specified number of milliseconds.

