# Texting

A component that will, when the SendMessage method is called, send the text message specified in the Message property to the phone number specified in the PhoneNumber property.

If the ReceivingEnabled property is set to 1 messages will not be received. If ReceivingEnabled is set to 2 messages will be received only when the application is running. Finally if ReceivingEnabled is set to 3, messages will be received when the application is running and when the application is not running they will be queued and a notification displayed to the user.

When a message arrives, the MessageReceived event is raised and provides the sending number and message.

An app that includes this component will receive messages even when it is in the background (i.e. when it's not visible on the screen) and, moreso, even if the app is not running, so long as it's installed on the phone. If the phone receives a text message when the app is not in the foreground, the phone will show a notification in the notification bar. Selecting the notification will bring up the app. As an app developer, you'll probably want to give your users the ability to control ReceivingEnabled so that they can make the phone ignore text messages.

If the GoogleVoiceEnabled property is true, messages can be sent over Wifi using Google Voice. This option requires that the user have a Google Voice account and that the mobile Voice app is installed on the phone. The Google Voice option works only on phones that support Android 2.0 (Eclair) or higher.

To specify the phone number (e.g., 650-555-1212), set the PhoneNumber property to a Text string with the specified digits (e.g., 6505551212). Dashes, dots, and parentheses may be included (e.g., (650)-555-1212) but will be ignored; spaces may not be included.

Another way for an app to specify a phone number would be to include a PhoneNumberPicker component, which lets the users select a phone numbers from the ones stored in the the phone's contacts.

---

### Properties

#### GoogleVoiceEnabled

If true, then SendMessage will attempt to send messages over Wifi using Google Voice. This requires that the Google Voice app must be installed and set up on the phone or tablet, with a Google Voice account. If GoogleVoiceEnabled is false, the device must have phone and texting service in order to send or receive messages with this component.

#### Message

The message that will be sent when the SendMessage method is called.

#### PhoneNumber

The number that the message will be sent to when the SendMessage method is called. The number is a text string with the specified digits (e.g., 6505551212). Dashes, dots, and parentheses may be included (e.g., (650)-555-1212) but will be ignored; spaces should not be included.

#### ReceivingEnabled

If set to 1 (OFF) no messages will be received. If set to 2 (FOREGROUND) or3 (ALWAYS) the component will respond to messages if it is running. If theapp is not running then the message will be discarded if set to 2(FOREGROUND). If set to 3 (ALWAYS) and the app is not running the phone willshow a notification. Selecting the notification will bring up the appand signal the MessageReceived event. Messages received when the appis dormant will be queued, and so several MessageReceived events mightappear when the app awakens. As an app developer, it would be a good idea to give your users control over this property, so they can maketheir phones ignore text messages when your app is installed.

---

### Events

#### MessageReceived(text number, text messageText)

Event that's raised when a text message is received by the phone.

---

### Methods

#### SendMessage()

Send a text message
