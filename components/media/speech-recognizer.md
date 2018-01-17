# SpeechRecognizer

Use a speech recognizer component to listen to the user speaking and convert the spoken sound into text using Android's speech recognition feature.

---

### Properties

#### Result

The last text produced by the recognizer.

---

### Methods

#### GetText()

Asks the user to speak, and converts the speech to text. Signals the AfterGettingText event when the result is available.

---

### Events

#### AfterGetting(Text result)

Signaled after the recognizer has produced text. The argument is the text result that was produced.

#### BeforeGettingText()

Signaled just before the recognizer is called.
