# Image Picker

A special-purpose button. When the user taps an image picker, the device's image gallery appears, and the user can choose an image. After an image is picked, it is saved, and the Selected property will be the name of the file where the image is stored. In order to not fill up storage, a maximum of 10 images will be stored. Picking more images will delete previous images, in order from oldest to newest.

## Properties

### BackgroundColor

Returns the button's background color

### Enabled

### FontBold \(designer only\)

### FontItalic \(designer only\)

### FontSize \(designer only\)

### FontTypeface \(designer only\)

### Height

### Image

Specifies the path of the button's image. If there is both an Image and a BackgroundColor, only the Image will be visible.

### Selection

Path to the file containing the image that was selected.

### Shape \(designer only\)

Specifies the button's shape \(default, rounded, rectangular, oval\). The shape will not be visible if an Image is being displayed.

### ShowFeedback

Specifies if a visual feedback should be shown for a button that as an image as background.

### Text

### TextAlignment \(designer only\)

### TextColor

### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

### Width

## Events

### AfterPicking\(\)

Simple event to be raised after the picker activity returns its result and the properties have been filled in.

### BeforePicking\(\)

Simple event to raise when the component is clicked but before the picker activity is started.

### GotFocus\(\)

Indicates the cursor moved over the button so it is now possible to click it.

### LostFocus\(\)

Indicates the cursor moved away from the button so it is now no longer possible to click it.

## Methods

### Open\(\)

Opens the picker, as though the user clicked on it.

