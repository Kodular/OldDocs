# Camcorder

A component to record a video using the device's camcorder.After the video is recorded, the name of the file on the phone containing the clip is available as an argument to the AfterRecording event. The file name can be used, for example, to set the source property of a VideoPlayer component.

## Properties

none

## Events

### AfterRecording\(text clip\)

Indicates that a video was recorded with the camera and provides the path to the stored picture.

## Methods

### RecordVideo\(\)

Records a video, then raises the AfterRecoding event.

