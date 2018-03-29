# Camera

Use a camera component to take a picture on the phone.

Camera is a non-visible component that takes a picture using the device's camera. After the picture is taken, the path to the file on the phone containing the picture is available as an argument to the AfterPicture event. The path can be used, for example, as the Picture property of an Image component.

## Properties

none

## Methods

### TakePicture\(\)

Opens the phone's camera to allow a picture to be taken.

## Events

### AfterPicture\(Text image\)

Called after the picture is taken. The text argument image is the path that can be used to locate the image on the phone.

