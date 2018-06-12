# Web Viewer

Component for viewing Web pages. The Home URL can be specified in the Designer or in the Blocks Editor. The view can be set to follow links when they are tapped, and users can fill in Web forms. Warning: This is not a full browser. For example, pressing the phone's hardware Back key will exit the app, rather than move back in the browser history.

You can use the WebViewer.WebViewString property to communicate between your app and Javascript code running in the Webviewer page. In the app, you get and set WebViewString. In the WebViewer, you include Javascript that references the window.AppInventor object, using the methoods and setWebViewString\(text\).

For example, if the WebViewer opens to a page that contains the Javascript command   
document.write\("The answer is" + window.AppInventor.getWebViewString\(\)\);   
and if you set WebView.WebVewString to "hello", then the web page will show   
The answer is hello.   
And if the Web page contains Javascript that executes the command   
windowAppInventor.setWebViewString\("hello from Javascript"\),   
then the value of the WebViewString property will be   
hello from Javascript.

## Properties

### CurrentPageTitle

Title of the page currently viewed

### CurrentUrl

URL of the page currently viewed. This could be different from the Home URL if new pages were visited by following links.

### FollowLinks

Determines whether to follow links when they are tapped in the WebViewer. If you follow links, you can use GoBack and GoForward to navigate the browser history.

### Height

### HomeUrl

URL of the page the WebViewer should initially open to. Setting this will load the page.

### IgnoreSslError

Determine whether or not to ignore SSL errors. Set to true to ignore errors. Use this to accept self signed certificates from websites.

### PromptforPermission

If True, then prompt the user of the WebView to give permission to access the geolocation API. If False, then assume permission is granted.

### UsesLocation \(designer only\)

Whether or not to give the application permission to use the Javascript geolocation API. This property is available only in the designer.

### Visible

Specifies whether the component should be visible on the screen. Value is true if the component is showing and false if hidden.

### WebViewString

Gets the WebView's String, which is viewable through Javascript in the WebView as the window.AppInventor object

### Width

## Events

none

## Methods

### boolean CanGoBack\(\)

Returns true if the WebViewer can go back in the history list.

### boolean CanGoForward\(\)

Returns true if the WebViewer can go forward in the history list.

### ClearCaches\(\)

Clear the WebViewer caches

### ClearLocations\(\)

Clear stored location permissions.

### GoBack\(\)

Go back to the previous page in the history list. Does nothing if there is no previous page.

### GoForward\(\)

Go forward to the next page in the history list. Does nothing if there is no next page.

### GoHome\(\)

Loads the home URL page. This happens automatically when the home URL is changed.

### GoToUrl\(text url\)

Load the page at the given URL.

