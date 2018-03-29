# Activity Starter

A component that can launch an activity using the `StartActivity` method.

Activities that can be launched include:

* Starting another App Inventor for Android app. To do so, first      find out the _class_ of the other application by downloading the source code and using a file explorer or unzip utility to find a file named "youngandroidproject/project.properties".

  The first line of the file will start with "main=" and be followed by the class name; for example, `main=com.makeroid.pavitra.HelloWorld.Screen1`.

  To make your `ActivityStarter` launch this application, set the      following properties:

  * `ActivityPackage` to the class name, dropping the last component \(for example, `com.gmail.Bitdiddle.Ben.HelloPurr`\)
  * `ActivityClass` to the entire class name \(for example, `com.gmail.Bitdiddle.Ben.HelloPurr.Screen1`\)

* Starting the camera application by setting the following      properties:
  * `Action`: `android.intent.action.MAIN`
  * `ActivityPackage`: `com.android.camera`
  * `ActivityClass`: `com.android.camera.Camera`
* Performing web search.  Assuming the term you want to search      for is "vampire" \(feel free to substitute your own choice\), set the properties to:
  * `Action`: `android.intent.action.WEB_SEARCH`
  * `ExtraKey`: query
  * `ExtraValue`: vampire
  * `ActivityPackage`: `com.google.android.providers.enhancedgooglesearch`
  * `ActivityClass`: `com.google.android.providers.enhancedgooglesearch.Launcher`
* Opening a browser to a specified web page. Assuming the page you want to go to is "www.facebook.com" \(feel free to substitute      your own choice\), set the properties to:
  * `Action`: `android.intent.action.VIEW`
  * `DataUri`: `http://www.facebook.com`

## Properties

### Action

### ActivityClass

### ActivityPackage

### DataType

### DataUri

### ExtraKey

Returns the extra key that will be passed to the activity.  
DEPRECATED: New code should use Extras property instead.

### ExtraValue

Returns the extra value that will be passed to the activity.  
DEPRECATED: New code should use Extras property instead.

### Extras

### Result

### ResultName

### ResultType

### ResultUri

## Events

### ActivityCanceled

Event raised if this ActivityStarter returns because the activity was canceled.

### AfterActivity

| Parameter | Type |
| :--- | :--- |
| result | text |

Event raised after this ActivityStarter returns.

## Methods

### ResolveActivity

#### Returns: \(text\)

Returns the name of the activity that corresponds to this ActivityStarter, or an empty string if no corresponding activity can be found.

### StartActivity

Start the activity corresponding to this ActivityStarter.

