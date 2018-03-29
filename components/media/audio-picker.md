# Audio Picker

A special-purpose button. When the user taps an audio picker, the device's audio gallery appears, and the user can choose an audio file. After an audio file is picked, it is saved, and the `Selected` property will be the name of the file where the audio file is stored. In order to not fill up storage, a maximum of 10 audio files will be stored.  Picking more audio files will delete previous audio files, in order from oldest to newest.

## Properties

### BackgroundColor

Returns the button's background color

### Enabled

If set, user can tap check box to cause action.

### FontBold

If set, button text is displayed in bold.

### FontItalic

If set, button text is displayed in italics.

### FontSize

Point size for button text.

### FontTypeface \(designer only\)

Font family for button text.

### FontTypefaceImport

Set a custom font.

### Height

### HeightPercent

### Image

Image to display on button.

### Selection

Path to the file containing the audio file that was selected.

### Shape \(designer only\)

Specifies the button's shape \(default, rounded, rectangular, oval\). The shape will not be visible if an Image is being displayed.

### ShowFeedback

Specifies if a visual feedback should be shown  for a button that as an image as background.

### Text

Text to display on button.

### TextAlignment \(designer only\)

Left, center, or right.

### TextColor

Color for button text.

### TouchColor

### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

### Width

### WidthPercent

## Events

### AfterPicking

Event to be raised after the picker activity returns its  
 result and the properties have been filled in.

### BeforePicking

Event to raise when the button of the component is clicked or the list is shown  
 using the Open block.  This event occurs before the list of items is displayed, and  
 can be used to prepare the list before it is shown.

### GotFocus

Indicates the cursor moved over the button so it is now possible to click it.

### LostFocus

Indicates the cursor moved away from the button so it is now no longer possible to click it.

### TouchDown

Indicates that the button was pressed down.

### TouchUp

Indicates that a button has been released.

## Methods

### Open

Opens the picker, as though the user clicked on it.

