# File

Non-visible component for storing and retrieving files. Use this component to write or read files on your device. The default behavior is to write files to the private data directory associated with your App. The Companion writes files to /sdcard/Makeroid/data for easy debugging. If the file path starts with a slash \(/\), then the file is created relative to /sdcard. For example, writing a file to /myFile.txt will write the file in /sdcard/myFile.txt.

## Properties

none

## Events

### GotText\(text text\)

Event indicating that the contents from the file have been read.

## Methods

### AppendToFile\(text text, text fileName\)

Appends text to the end of a file. Creates the file if it does not already exist. See the help text under SaveFile for information about where files are written.

### Delete\(text fileName\)

Deletes a file from storage. Prefix the filename with / to delete a specific file in the SD card \(for example, /myFile.txt will delete the file /sdcard/myFile.txt\). If the filename does not begin with a /, then the file located in the program's private storage will be deleted. Starting the file with // is an error because asset files cannot be deleted.

### ReadFrom\(text fileName\)

Reads text from a file in storage. Prefix the filename with / to read from a specific file on the SD card \(for example, /myFile.txt will read the file /sdcard/myFile.txt\). To read assets packaged with an application \(also works for the Companion\) start the filename with // \(two slashes\). If a filename does not start with a slash, it will be read from the application's private storage \(for packaged apps\) and from /sdcard/Makeroid/data for the Companion.

### SaveFile\(text text, text fileName\)

Saves text to a file. If the filename begins with a slash \(/\) the file is written to the sdcard \(for example, writing to /myFile.txt will write the file to /sdcard/myFile.txt\). If the filename does not start with a slash, it will be written in the program's private data directory where it will not be accessible to other programs on the phone. There is a special exception for the Makeroid Companion where these files are written to /sdcard/Makeroid/data to facilitate debugging. Note that this block will overwrite a file if it already exists. If you want to add content to a file use the append block.

