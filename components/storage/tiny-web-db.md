# Tiny Web DB

Non-visible component that communicates with a Web service to store and retrieve information.

See [Creating a Custom TinyWebDB Service.](http://ai2.appinventor.mit.edu/reference/other/tinywebdb.html)

## Properties

### ServiceURL

The URL to the database with which the component should communicate.

## Events

### GotValue\(text tagFromWebDB, any valueFromWebDB\)

Indicates that a GetValue server request has succeeded.

### ValueStored\(\)

Event indicating that a StoreValue server request has succeeded.

### WebServiceError\(text message\)

Indicates that the communication with the Web service signaled an error.

## Methods

### GetValue\(text tag\)

Sends a request to the Web service to get the value stored under the given tag. The Web service must decide what to return if there is no value stored under the tag. This component accepts whatever is returned.

### StoreValue\(text tag, any valueToStore\)

Sends a request to the Web service to store the given value under the given tag.

