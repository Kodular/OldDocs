# Phone Number Picker

A button that, when clicked on, displays a list of the contacts' phone numbers to choose among. After the user has made a selection, the following properties will be set to information about the chosen contact:

* ContactName: the contact's name
* PhoneNumber: the contact's phone number
* EmailAddress: the contact's email address
* Picture: the name of the file containing the contact's image, which can be used as a Picture property value for the Image or ImageSprite component.

Other properties affect the appearance of the button (TextAlignment, BackgroundColor, etc.) and whether it can be clicked on (Enabled).

The PhoneNumberPicker component may not work on all Android devices. For example, on Android systems before system 3.0, the returned lists of phone numbers and email addresses will be empty.

---

### Properties

#### BackgroundColor

Returns the button's background color

#### ContactName

#### EmailAddress

#### Enabled

#### FontBold (designer only)

#### FontItalic (designer only)

#### FontSize (designer only)

#### FontTypeface (designer only)

#### Height

#### Image

Specifies the path of the button's image. If there is both an Image and a BackgroundColor, only the Image will be visible.

#### PhoneNumber

#### Picture

#### Shape (designer only)

Specifies the button's shape (default, rounded, rectangular, oval). The shape will not be visible if an Image is being displayed.

#### ShowFeedback

Specifies if a visual feedback should be shown for a button that as an image as background.

#### Text

TextAlignment (designer only)

#### TextColor

#### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

#### Width

---

### Events

#### AfterPicking()

Simple event to be raised after the picker activity returns its result and the properties have been filled in.

#### BeforePicking()

Simple event to raise when the component is clicked but before the picker activity is started.

#### GotFocus()

Indicates the cursor moved over the button so it is now possible to click it.

#### LostFocus()

Indicates the cursor moved away from the button so it is now no longer possible to click it.

---

### Methods

#### Open()

Opens the picker, as though the user clicked on it.
