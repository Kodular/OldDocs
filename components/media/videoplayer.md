# VideoPlayer

A multimedia component capable of playing videos. When the application is run, the VideoPlayer will be displayed as a rectangle on-screen. If the user touches the rectangle, controls will appear to play/pause, skip ahead, and skip backward within the video. The application can also control behavior by calling the Start, Pause, and SeekTo methods.

Video files should be in 3GPP (.3gp) or MPEG-4 (.mp4) formats. For more details about legal formats, see Android Supported Media Formats.

Makeroid only permits video files under 1 MB and limits the total size of an application to 5 MB, not all of which is available for media (video, audio, and sound) files. If your media files are too large, you may get errors when packaging or installing your application, in which case you should reduce the number of media files or their sizes. Most video editing software, such as Windows Movie Maker and Apple iMovie, can help you decrease the size of videos by shortening them or re-encoding the video into a more compact format.

You can also set the media source to a URL that points to a streaming video, but the URL must point to the video file itself, not to a program that plays the video.

---

### Properties

#### FullScreen

#### Height

#### Source

The "path" to the video. Usually, this will be the name of the video file, which should be added in the Designer.

#### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

#### Volume

Sets the volume to a number between 0 and 100. Values less than 0 will be treated as 0, and values greater than 100 will be treated as 100.

#### Width

---

### Events

#### Completed()

Indicates that the video has reached the end

---

### Methods

#### GetDuration()

Returns duration of the video in milliseconds.

#### Pause()

Pauses playback of the video. Playback can be resumed at the same location by calling the Start method.

#### SeekTo(number ms)

Seeks to the requested time (specified in milliseconds) in the video. If the video is paused, the frame shown will not be updated by the seek. The player can jump only to key frames in the video, so seeking to times that differ by short intervals may not actually move to different frames.

#### Start()

Starts playback of the video.
