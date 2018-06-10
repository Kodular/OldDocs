# Release Notes

## 3.0.0 _Beta_

`25 Dec, 2017`

* **New Components**
  * Created SurfaceView Component in User Interface category
  * Created VideoPicker Component in Media category
  * Created LeadBolt Component in Monetization category
  * Created Space Component in Layout category
  * Created Notification Component in Experimental category
  * Created CloudDB Component in Experimental category
  * Created DeviceTools Component in new Device category
  * Created Wallpaper Component in new Device category
  * Created Audio Component in new Device category
  * Created Package Component in new Device category
  * Created Screenshot Component in new Device category
  * Created GoogleShortlink Component in new Google category
* **New Events**
  * Added to Screen OnAppResume Event
  * Added to Screen OnAppPause Event
  * Added to Screen OnAppStop Event
  * Added to TextBox OnTextChanged Event
  * Added to Download GotFileSize Event
  * Added to Download DownloadComplete Event return options now FileSize, Name and Path
  * Added to Notifier AfterMessageDialog Event \(for Custom Choose Dialog\)
* **New Properties**
  * Added to Screen About Screen Title Property
  * Added to Screen Show Options Menu Property \(Hide or show the 3 Dots Menu\)
  * Added to TextBox TextLength Property
  * Added to TextBox CurrentPosition Property
  * Added to All Layouts is Card Property
  * Added to VideoPlayer Volume Property
  * Added to VideoPlayer IsPlaying Property
  * Added to VideoPlayer CurrentPosition Property
* **New Functions**
  * Added to Screen Task Description Function
  * Added to TextBox SetCursorAt Function
  * Added to TextBox SetCursorAtEnd Function
  * Added to Download GetFileSize Function
* **Bugs Fixed**
  * Fixed some upper case camels
  * Fixed Network issue \(Null pointer exceptions on some Android 5 devices\)
  * Fixed Network issue \(“IsConnected” block was not correct working\)
  * Fixed ListView issue \(change text size was not possible\)
  * Fixed Switch bug \(bold, italic was not working\)
  * Fixed Textbox bug \(projects with checked “Numbers Only” in textbox were not importable\)
  * Fixed RadioButton bug \(text color was not working\)
  * Fixed Download bug \(there was something wrong with the properties\)
  * Fixed Menu Initialize event bug \(on screen orientation was all items removed\)
  * Fixed Spinner bug \(some letters was not full visible\)
  * Fixed Button bug \(Color NONE was not working for buttons with default shape option\)
* **Other Changes**
  * SET A CUSTOM PACKAGE NAME FOR YOUR APP \(thanks to AppyBuilder team\) \(Removed the PackageName input from NewProject dialog, set it from Screen1\) Instructions
  * Implemented PushNotifications inside the Builder, so users can subscribe to be up-to-date with latest Makeroid Announcements
  * Added \*.gif support \(animated images\) for Image Component
  * Added input type Phone Number to TextBox Component
  * Added support for Dragging and Dropping Components on mobile \(merged from Evan’s PullRequest\)
  * Moved GoogleMap Component to new Google category
  * Moved GoogleAccount Component to new Google category
  * Updated Translations from Makeroid Translation Center
* **File Component Update**
  * Added New Methods to File component:
    * Move
    * GetTotalSpace
    * GetFreeSpace
    * Exists
    * FileSize
    * Copy
    * GetFileName
    * IsFile
    * IsDirectory
* **UI Update**
  * Designer now provides draggable text-entry for entering text in the following Components:
  * Qr Code
    * ListView \(elements from string\)
    * TextBox
    * Checkbox
    * Label
    * RadioButton
    * Switch
  * Redesigned Components Palette: Now there is a table with all components instead of a list
  * Added Scrollbars to different boxes to enhance user experience
* **Companion Changes**
  * Compressed Images Size \(which probably was causing the “Companion stopped working” error\)
  * Added MultiLanguage Support \(detected automatically from Device’s language\)

## 2.2.0 _Beta_

`12 Nov, 2017`

* **New Components**
  * Created SQLite Component by @CarlosPedroza27
  * Created Download Component
  * Created Fingerprint Component
  * Created SoundSensor Component
  * Created GoogleAccountPicker Component \(check this thread\)
  * Moved Firebase from Experimental to Storage category
* **New Properties**
  * Added to VideoPlayer new property show/hide the control button blocks
  * Added to WebViewer new property Use External Browser
  * Added to WebViewer new property Scrollbar
  * Added to ScrollableArrangements new property Scrollbar
  * Added to Screen new property is Keyboard Visible
  * Added to Slider new property Thumb Color
  * Added to Slider new property Thumb Image
  * Added to Player new property Current Position
  * Added to Player new property Duration
  * Added to Player new property Get TrackInfo
  * Added to Player new property Volume
  * Added to OCR new property Return Only Message
  * Added to Buttons new function Border Shadow \(for Android 5+\)
  * Added to TextBox new function Decimal number and Phone Number
  * Added to PushNotifications new function Enable Log
  * Added to PushNotifications new function Enable Sound
  * Added to PushNotifications new function Enable Vibration
  * Added to PushNotifications new property Get Permission Status
  * Added to PushNotifications new property Get Subscription Status
  * Added to PushNotifications new property Get User Id
  * Added to PushNotifications new property Get Permission Status
  * Added to PushNotifications new function Set Subscription
* **New Events**
  * Added to WebViewer new event Progress Changed
  * Added to WebViewer new event Cookies Removed
* **New Functions**
  * Added to WebViewer new function Clear Cookies
  * Added to BluetoothClient new function Remove Name From Address
  * Added to Player new function Seek To
  * Added to Firebase new functions Go Online & Go Offline
  * Added to Google Maps new functions Add Polyline, Remove Polyline & Update Polyline
* **Other Updates**
  * Notifier Update based on @vishwasadiga Dialogs Extension
    * New property Light Theme
    * New function Show Lightbox
    * New event Lightbox Closed
    * New function Show Radio List Dialog
    * New event Radio Selection
    * New function Show Checkbox List Dialog
    * New event Checkbox Selection
    * New function Show List Picker
    * New event List Picker Selection
    * New function Show Image Dialog
    * New event Image Dialog Close
    * New function Show Number Picker
    * New event Number Picker Selection
    * New function Show Word Picker
    * New event Word Picker Selection
    * New function Custom Choose Dialog
    * New event Got Custom Choose Dialog
    * New function Custom Message Dialog
    * New function Show Text Input Dialog
    * New event Got Text Input From Dialog
    * New function Update Progress
    * New function Show Spinning Progress
    * New function Show Linear Progress
    * New function Dismiss Spinning Progress
    * Now assets are saved at /Makeroid directory
  * Enabled for WebViewer setAllowFileAccess8 and setAllowContentAccess5
* **Companion Changes**
  * Fixed Companion stopped working error
  * Fixed Status Tab which wasn’t showing the Status Site
  * Added AdMob Banner at Testing Tab \(our servers costs have increased and we have to pay them :sweat\_smile:\)
* **Bugs Fixed**
  * Fixed VideoPlayer bug - Now you can play videos from external URL
  * Fixed WebViewer bug - URL Loading
  * Fixed Slider bug - When Disabled &gt; Ugly Slider
  * Fixed Spinner bug - Item Background Color crashed on devices below API 16. Now it works too for all APIs below 16
  * Fixed Player bug - Load files from assets was not working

## 2.1.1 _Beta_

`7 Oct, 2017`

* Event to receive OCR Server Status
* Function to call the new OCR Event
* New Sharing Features:
  * Event AppNotFound
  * Function ShareMessage to:
    * Facebook
    * FacebookMessenger
    * Twitter
    * Telegram
    * Google+
    * SnapChat
    * WhatsApp
  * Property ShareDialogMessage
* Fixed PopupPanel position in Chrome
* Updated Translations
* Fixed Companion for Live Testing
* Fixed QR Code Screen

## 2.1.0 _Beta_

`1 Oct, 2017`

* **New Components**
  * Made Billing component visible for everyone
* **New Features**
  * New Hint Color Property for Textbox
  * Hide Border on Buttons for devices with API &gt;= 21
  * YandexTranslate updated with new ApiKey property
  * ListPicker V2 with Material Design
  * New methods to set and get the text size in Switch, Radiobutton, ListView and Spinner
  * Item Height in % for ListView
  * Added HighlightColor on Textbox
  * Added TitlebarTextColor property
  * Show TitlebarBackButton method added
  * Implemented Touch Color Property for Buttons with \_Android &gt;= 5
  * TitleBar Subtitle has HTML Support now
  * Created new default fonts \(roboto thin, roboto regular, font awesome, material icons\)
  * Added Canvas Fonts & Scale Property
  * Made clickable arrangements \(horizontal, horizontal scroll, vertical & vertical scroll layouts\)
  * New OCR properties: CreateSearchablePdf & ReturnOnlyPdfLink
  * New Notifier/ Toast functions: Change the text color and the background of a toast message
* **Important Changes**
  * OptionMenus must now be added with a ‘make a list’ block. Remember to update the blocks in your apps using this function created before the update.
  * Removed “Prompt” in Spinner and added new property for spinner “Use Prompt” and “Prompt Item Color”
  * Removed NumbersOnly property on the TextBox
* **UI Updates**
  * Added a beautiful Night Theme to the builder to help Makers that like to code during the night
  * Added a new ColorPicker to set custom colours
  * Added DropFileToUpload in Assets
  * Added MediaPreview in Assets
  * Made FloatingBox draggable
* **Live Testing**
  * We have just added an ad to the Status tab in the companion, which newer version can be downladed here We hope to have an automatic update feature in the next version of it
  * The Makeroid Starter has the same version. There’s no need to update it
* **Bugs fixed**
  * The team has fixed lots of bugs that were reported here and through the Support Chat Thanks to all those who helped us catch and fix those pesky errors!
  * Fixed some design bugs on the designer, concretly on the phone screen
  * Fixed Firebase bug that crashes apps
  * Added default Android Animation in all button’s shapes

## 2.0.0 _Beta_

`4 Sep, 2017`

* **New Components**
  * **Floating Action Button** Use in your app to have a primary button and bring a more professional Material Design
  * **Ads Components** \(_AdMob_\)
    * AdMob Banner: A simple banner to place ads
    * AdMob Interstitial: Show an add in all screen that can be dismissable by user
    * AdMob RewardedVide: The same as the Interstitial, but with a video
  * **New Sensors**
    * Magnetic Field Sensor: Detect all magnetic forces with it \(useful to be used with compass\)
    * Preassure Sensor: Get air pressure with your app
    * Temperature Sensor: Find current temperature and make your weather app
  * **Network Component:** Place it in your app if you need users to be online always
  * **QR Component:** Generate a QR Code from your app
  * **OCR Component:** The famous OCR system can be now integrated in your app
  * **WiFi Component:** Get information from the Wifi connection if avaliable
* **New Properties**
  * **Switcher Update:** Now there are more properties that can be customizable with the switcher
  * **Spinner Update:** Also, some more features have been added to it
  * **RadioButton Update:** Enhanced some properties and added new ones
  * **Textbox Changes**
    * **Normal Textbox**: Now there is a dropdown to choose the input type \(ie.: normal, password, numeric...\) plus added a LineColor property
    * **Password Texbox**: Has been hidden from the Palette in order to use the Normal Textbox
  * **Listview Properties:** Added some new properties to improve our ListView usage
* **New Features**
  * **Simulate Click Button:** Simulate a button click from blocks
  * **Custom Fonts:** Custom fonts avaliable in lots of components
  * **HTML Support:** Added HTML markup in listview, switch, radio button and buttons
* **Builder Changes**
  * **Some design updates**
    * Added phone's frame
    * Added animations in the palette
    * Improved some elements with Material Design
    * Fixed bug that allows to create duplicated projects or containing spaces
  * **New TermsOfService:** We updated the ToS to the 21th century adding some reasons of why an account can be suspended
  * **Original Package Name support for Google Play Store**
    * [See this topic for how to use it](https://community.makeroid.io/t/how-to-use-the-special-package-names/296)
* **Live Testing**
  * **Changed Companion PackageName** to `com.makeroid.companion`
    * [See this for further information](https://community.makeroid.io/t/new-domain-makeroid-io/276/6)
  * **Updated Makeroid Starter to work with new Companion**
  * **Fixed error that made the Companion to not start on Android &lt;5.0**

> _**Note:** Remember to update the_ [_Starter_](https://github.com/Makeroid/Starter/releases/latest) _and the_ [_Companion_](https://rink.hockeyapp.net/apps/93f5fed412b2457296f351cd0f1d824e/#) _to latest version_

* **Bugs Fixed**
  * **Fixed bug that buttons weren't clickable on some Android devices under 5.0**
  * **Fixed button size and color issue**
  * **WebViewer URL Fix:** Now it's not necessary to include the _http_ part when trying to open an external URL; it's detected automatically

## 1.3.1 _Beta_

`15 Aug, 2017`

* `NEW Component` Radio Button 
* `NEW Component` Rating Bar 
* `NEW Component` Metadata Component 
* `NEW Feature` Pull down to refresh in WebViewer 
* `UPDATE` Added USB Connection button - We are working on the client side 
* `FIXED` Minor bugs fixed

## 1.2.1 _Beta_

`07 Aug 2017`

* `NEW` Version nomenclature 
* `NEW` Push Notifications component with OneSignal 
* `NEW` Switch component 
* `UPDATE` Add property to change checkbox color 
* `IMPROVEMENT` Now we will send you notifications from the Companion of updates or important notes 
* `FIXED` Some links that were pointing to 404 
* `FIXED` Minor bugs fixed 

## 1.1.1 _Beta_

`03 Aug 2017`

* `NEW` Released Companion
* `NEW` New version tagging
* `UPDATE` New logos!
* `UPDATE` Option to set clickable components \(image & label\)
* `UPDATE` Change default StatusBar and TitleBar colors
* `FIXED` Some bugs

## 0.3.1 _Beta_

`01 Aug 2017`

* `NEW` Added option to change tab in blocks
* `NEW` Reset the custom menu from blocks
* `NEW` Added this Release Notes
* `IMPROVED` Static files
* `FIXED` Textboxes that can be resized became rounded
* `FIXED` Random error in Background Color to some components

## 0.2.1 Beta

`25 Jul 2017`

* `NEW` Added an amazing Material Design to the builder
* `IMPROVED` Build server
* `FIXED` Crash on load to built apps

## 0.1.1 _Beta_

`23 Jul 2017`

* `NEW` This is our first version There can be lots of bugs

