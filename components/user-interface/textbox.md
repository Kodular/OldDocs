# TextBox

Users enter text in a text box component.

The initial or user-entered text value in a text box component is in the Text property. If Text is blank, you can use the Hint property to provide the user with a suggestion of what to type. The Hint appears as faint text in the box.

The MultiLine property determines if the text can have more than one line. For a single line text box, the keyboard will close automatically when the user presses the Done key. To close the keyboard for multiline text boxes, the app should use the HideKeyboard method or rely on the user to press the Back key.

The NumbersOnly property restricts the keyboard to accept numeric input only.

Other properties affect the appearance of the text box \( TextAlignment , BackgroundColor , etc.\) and whether it can be used \( Enabled \).

Text boxes are usually used with the Button component, with the user clicking on the button when text entry is complete.

If the text entered by the user should not be displayed, use PasswordTextBox instead.

## Methods

### HideKeyboard\(\)

Hide the keyboard. Only multiline text boxes need this. Single line text boxes close the keyboard when the users presses the Done key.

### RequestFocus\(\)

Sets the textbox active.

## Properties

### BackgroundColor

The background color of the input box. You can choose a color by name in the Designer or in the Blocks Editor. The default background color is 'default' \(shaded 3-D look\).

### Enabled

Whether the user can enter text into this input box. By default, this is true.

### FontBold \(designer only\)

Whether the font for the text should be bold. By default, it is not.

### FontItalic \(designer only\)

Whether the text should appear in italics. By default, it does not.

### FontSize

The font size for the text. By default, it is 14.0 points.

### FontTypeface \(designer only\)

The font for the text. The value can be changed in the Designer.

### Height

### Hint

Text that should appear faintly in the input box to provide a hint as to what the user should enter. This can only be seen if the Text property is empty.

### MultiLine

If true, then this text box accepts multiple lines of input, which are entered using the return key. For single line text boxes there is a Done key instead of a return key, and pressing Done hides the keyboard. The app should call the HideKeyboard method to hide the keyboard for a mutiline text box.

### NumbersOnly

If true, then this text box accepts only numbers as keyboard input. Numbers can include a decimal point and an optional leading minus sign. This applies to keyboard input only. Even if NumbersOnly is true, you can use \[set Text to\] to enter any text at all.

### Text

The text in the input box, which can be set by the programmer in the Designer or Blocks Editor, or it can be entered by the user \(unless the Enabled property is false\).

### TextAlignment \(designer only\)

Whether the text should be left justified, centered, or right justified. By default, text is left justified.

### TextColor

The color for the text. You can choose a color by name in the Designer or in the Blocks Editor. The default text color is black.

### Visible

Whether the component is visible

### Width

## Events

### GotFocus\(\)

Event raised when this component is selected for input, such as by the user touching it.

### LostFocus\(\)

Event raised when this component is no longer selected for input, such as if the user touches a different text box.

