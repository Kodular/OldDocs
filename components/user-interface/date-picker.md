# DatePicker

A button that, when clicked on, launches a popup dialog to allow the user to select a date.

---

### Properties

##### BackgroundColor

![](/assets/user-interface/date-picker/Properties/background-color.png)

Returns the button's background color

##### Day

the Day of the month that was last picked using the DatePicker.

##### Enabled

![](/assets/user-interface/date-picker/Properties/enabled.png)

If set, user can tap check box to cause action.

##### FontBold

![](/assets/user-interface/date-picker/Properties/font-bold.png)

If set, button text is displayed in bold.

##### FontItalic

![](/assets/user-interface/date-picker/Properties/font-italic.png)

If set, button text is displayed in italics.

##### FontSize

![](/assets/user-interface/date-picker/Properties/font-size.png)

Point size for button text.

##### FontTypeface \(designer only\)

![](/assets/user-interface/date-picker/Properties/font-typeface-set.png)

Font family for button text.

##### Height

![](/assets/user-interface/date-picker/Properties/height.png)

To set it's height.

##### Image

![](/assets/user-interface/date-picker/Properties/image.png)

Image to display on button.

##### Instant

Instant of date. This instant can be used with [Clock](http://ai2.appinventor.mit.edu/reference/components/sensors.html#Clock)

component for date documentation, conversion, and matriculation.

##### Month

the number of the Month that was last picked using the DatePicker. Note that months start in 1 = January, 12 = December.

##### MonthInText

Returns the name of the Month that was last picked using the DatePicker, in textual format.

##### Shape \(designer only\)

Specifies the button's shape \(default, rounded, rectangular, oval\). The shape will not be visible if an Image is being displayed.

##### ShowFeedback

![](/assets/user-interface/date-picker/Properties/show-feedback.png)

Specifies if a visual feedback should be shown for a button that as an image as background.

##### Text

![](/assets/user-interface/date-picker/Properties/text.png)

Text to display on button.

##### TextAlignment \(designer only\)

Left, center, or right.

##### TextColor

![](/assets/user-interface/date-picker/Properties/text-color.png)

Color for button text.

##### Visible

![](/assets/user-interface/date-picker/Properties/visible.png)

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

##### Width

![](/assets/user-interface/date-picker/Properties/width.png)

To set it's width.

##### Year

the Year that was last picked using the DatePicker

---

### Events

##### AfterDateSet

![](/assets/user-interface/date-picker/Events/after-date-set.png)

Event that runs after the user chooses a Date in the dialog

##### GotFocus

![](/assets/user-interface/date-picker/Events/got-focus.png)

Indicates the cursor moved over the button so it is now possible to click it.

##### LostFocus

![](/assets/user-interface/date-picker/Events/lost-focus.png)

Indicates the cursor moved away from the button so it is now no longer possible to click it.

##### TouchDown

![](/assets/user-interface/date-picker/Events/touch-down.png)

Indicates that the button was pressed down.

##### TouchUp

![](/assets/user-interface/date-picker/Events/touch-up.png)

Indicates that a button has been released.

---

### Methods

##### LaunchPicker

![](/assets/user-interface/date-picker/Methods/launch-picker.png)

Launches the DatePicker popup.

##### SetDateToDisplay

![](/assets/user-interface/date-picker/Methods/set-date-to-display.png)

###### Parameters: \(number year, number month, number day\)

Allows the user to set the date to be displayed when the date picker opens. Valid values for the month field are 1-12 and 1-31 for the day field.

##### SetDateToDisplayFromInstant

![](/assets/user-interface/date-picker/Methods/set-date-to-display-from-instant.png)

###### Parameter: \(InstantInTime instant\)

Allows the instant to set the year, month, and day to be displayed when the date picker opens. Instants are used in Clock, DatePicker, and TimePicker components.

