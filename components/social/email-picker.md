# Email Picker

An EmailPicker is a kind of text box. If the user begins entering the name or email address of a contact, the phone will show a dropdown menu of choices that complete the entry. If there are many contacts, the dropdown can take several seconds to appear, and can show intermediate results while the matches are being computed.

The initial contents of the text box and the contents< after user entry is in the Text property. If the Text property is initially empty, the contents of the Hint property will be faintly shown in the text box as a hint to the user.

Other properties affect the appearance of the text box (TextAlignment, BackgroundColor, etc.) and whether it can be used (Enabled).

Text boxes like this are usually used with Button components, with the user clicking on the button when text entry is complete.

---

### Methods

#### RequestFocus()

Sets the EmailPicker active.

---

### Properties

#### BackgroundColor

The background color of the input box. You can choose a color by name in the Designer or in the Blocks Editor. The default background color is 'default' (shaded 3-D look).

#### Enabled

Whether the user can enter text into this input box. By default, this is true.

#### FontBold (designer only)

Whether the font for the text should be bold. By default, it is not.

#### FontItalic (designer only)

Whether the text should appear in italics. By default, it does not.

#### FontSize

The font size for the text. By default, it is 14.0 points.

#### FontTypeface (designer only)

The font for the text. The value can be changed in the Designer.

#### Height

#### Hint

Text that should appear faintly in the input box to provide a hint as to what the user should enter. This can only be seen if the Text property is empty.

#### Text

The text in the input box, which can be set by the programmer in the Designer or Blocks Editor, or it can be entered by the user (unless the Enabled property is false).

#### TextAlignment (designer only)

Whether the text should be left justified, centered, or right justified. By default, text is left justified.

#### TextColor

The color for the text. You can choose a color by name in the Designer or in the Blocks Editor. The default text color is black.

#### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

#### Width

---

### Events

#### GotFocus()

Event raised when this component is selected for input, such as by the user touching it.

#### LostFocus()

Event raised when this component is no longer selected for input, such as if the user touches a different text box.

---

### Methods

none
