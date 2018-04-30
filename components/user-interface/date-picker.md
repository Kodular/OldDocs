---
description: >-
  A button that, when clicked on, launches a popup dialog to allow the user to
  select a date.
---

# Date Picker

## Properties

### BackgroundColor

![](../../.gitbook/assets/background-color.png)

Returns the button's background color

### Day

the Day of the month that was last picked using the DatePicker.

### Enabled

![](../../.gitbook/assets/enabled.png)

If set, user can tap check box to cause action.

### FontBold

![](../../.gitbook/assets/font-bold.png)

If set, button text is displayed in bold.

### FontItalic

![](../../.gitbook/assets/font-italic.png)

If set, button text is displayed in italics.

### FontSize

![](../../.gitbook/assets/font-size.png)

Point size for button text.

### FontTypeface \(designer only\)

![](https://github.com/makeroid/docs/tree/6b89ce9eb8c93762fd238491325318be0e89c35f/assets/user-interface/date-picker/Properties/font-typeface-set.png)

Font family for button text.

### Height

![](../../.gitbook/assets/height.png)

To set it's height.

### Image

![](../../.gitbook/assets/image.png)

Image to display on button.

### Instant

Instant of date. This instant can be used with [Clock](http://ai2.appinventor.mit.edu/reference/components/sensors.html#Clock)

component for date documentation, conversion, and matriculation.

### Month

the number of the Month that was last picked using the DatePicker. Note that months start in 1 = January, 12 = December.

### MonthInText

Returns the name of the Month that was last picked using the DatePicker, in textual format.

### Shape \(designer only\)

Specifies the button's shape \(default, rounded, rectangular, oval\). The shape will not be visible if an Image is being displayed.

### ShowFeedback

![](../../.gitbook/assets/show-feedback.png)

Specifies if a visual feedback should be shown for a button that as an image as background.

### Text

![](../../.gitbook/assets/text-1.png)

Text to display on button.

### TextAlignment \(designer only\)

Left, center, or right.

### TextColor

![](../../.gitbook/assets/text-color.png)

Color for button text.

### Visible

![](../../.gitbook/assets/visible.png)

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

### Width

![](../../.gitbook/assets/width-1.png)

To set it's width.

### Year

the Year that was last picked using the DatePicker

## Events

### AfterDateSet

![](../../.gitbook/assets/after-date-set.png)

Event that runs after the user chooses a Date in the dialog

### GotFocus

![](../../.gitbook/assets/got-focus.png)

Indicates the cursor moved over the button so it is now possible to click it.

### LostFocus

![](../../.gitbook/assets/lost-focus.png)

Indicates the cursor moved away from the button so it is now no longer possible to click it.

### TouchDown

![](../../.gitbook/assets/touch-down.png)

Indicates that the button was pressed down.

### TouchUp

![](../../.gitbook/assets/touch-up.png)

Indicates that a button has been released.

## Methods

### LaunchPicker

![](../../.gitbook/assets/launch-picker.png)

Launches the DatePicker popup.

### SetDateToDisplay

![](../../.gitbook/assets/set-date-to-display.png)

#### Parameters: \(number year, number month, number day\)

Allows the user to set the date to be displayed when the date picker opens. Valid values for the month field are 1-12 and 1-31 for the day field.

### SetDateToDisplayFromInstant

![](../../.gitbook/assets/set-date-to-display-from-instant.png)

#### Parameter: \(InstantInTime instant\)

Allows the instant to set the year, month, and day to be displayed when the date picker opens. Instants are used in Clock, DatePicker, and TimePicker components.

