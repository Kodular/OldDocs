# Time Picker

A button that, when clicked on, launches a popup dialog to allow the user to select a time.

---

### Properties

#### BackgroundColor

Returns the button's background color

#### Enabled

#### FontBold (designer only)

#### FontItalic (designer only)

#### FontSize (designer only)

#### FontTypeface (designer only)

#### Height

#### Hour

The hour of the last time set using the time picker. The hour is in a 24 hour format. If the last time set was 11:53 pm, this property will return 23.

#### Image

Specifies the path of the button's image. If there is both an Image and a BackgroundColor, only the Image will be visible.

#### Instant

Instant of time. This instant can be used with Clock component for time documentation, conversion, and matriculation.

#### Minute

The minute of the last time set using the time picker

#### Shape (designer only)

Specifies the button's shape (default, rounded, rectangular, oval). The shape will not be visible if an Image is being displayed.

#### ShowFeedback

Specifies if a visual feedback should be shown for a button that as an image as background.

#### Text

#### TextAlignment (designer only)

#### TextColor

#### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

#### Width

---

### Events

#### AfterTimeSet()

This event is run when a user has set the time in the popup dialog.

#### GotFocus()

Indicates the cursor moved over the button so it is now possible to click it.

#### LostFocus()

Indicates the cursor moved away from the button so it is now no longer possible to click it.

---

### Methods

#### LaunchPicker()

Launches the TimePicker popup.

#### SetTimeToDisplay(number hour, number minute)

Allows the user to set the time to be displayed when the time picker opens. Valid values for the hour field are 0-23 and 0-59 for the second field.

#### SetTimeToDisplayFromInstant(InstantInTime instant)

Allows the instant to set the hour and minute to be displayed when the time picker opens. Instants are used in Clock, DatePicker, and TimePicker components.
