# Create Extensions

This tutorial will guide you to create extensions for Makeroid.

> This guide assumes you to be a Windows user.

---

### Tools you will need:

* [App Inventor Sources ](https://github.com/mit-cml/appinventor-sources)
* [Java JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
* [Apache Ant](http://ant.apache.org/bindownload.cgi)
* [Git](https://git-scm.com/downloads) \(or [GitHub Desktop](https://desktop.github.com/)\)
* Java IDE/Text Editor \([Eclipse](http://www.eclipse.org/downloads/eclipse-packages/), [IntelliJ IDEA](https://www.jetbrains.com/idea/download/), [Notepad++](https://notepad-plus-plus.org), [Atom](https://atom.io/) are recommended\)

> **Download everything listed above and let's get started!**

### Step 1: Setting up Java JDK

* Install JDK

  > :warning: _Be sure not to install it in a directory whose path contains spaces_

* Set the Environmental Variables:

  * Set** **`JAVA_HOME` to where you installed Java JDK.

    For example: `C:\Program Files\Java\jdk1.8.0_131`

  * Edit** **`PATH` and add those:

    `%JAVA_HOME%/bin`, `%JAVA_HOME%/jre/bin`, `C:\ProgramData\Oracle\Java\javapath`

* **Check Java installation:** Execute `java -version`

  ```
    C:\Users\Pavitra>java -version
    java version "1.8.0_131"
    Java(TM) SE Runtime Environment (build 1.8.0_131-b11)
    Java HotSpot(TM) 64-Bit Server VM (build 25.131-b11, mixed mode)
  ```

### Step 2: Setting up Apache Ant

* Unzip the folder and move it to a place where it is safe. For example: `C:\apache-ant-1.10.1`

  > :warning: _Be sure not to place it in a directory whose path contains spaces_

* Set the Environmental Variables:

  * **Set **`ANT_HOME` to where you have the Ant folder placed. For example: `C:/Ant/apache-ant-1.10.1`

  * **Edit **`Path` and add `<Ant Directory>\bin`

    For example: `C:/Ant/apache-ant-1.10.1\bin`

  * **Edit **`ClassPath` and add `<Ant Directory>\bin`

    For example: `C:/Ant/apache-ant-1.10.1\lib`

* **Check Ant installation**: Execute `ant -version`

  ```
    C:\Users\Pavitra>ant -version
    Apache Ant(TM) version 1.10.1 compiled on February 2 2017
  ```

### Step 3: Setting up Git

* Set it up as written in this [tutorial](https://www.atlassian.com/git/tutorials/install-git#windows)

* **Check Git installation**: Execute `git version`

  ```
    C:\Users\Pavitra>git version
    git version 2.11.0.windows.3
  ```

### Step 4: App Inventor Sources

* Unzip the folder and move it to a place where it is safe

  > :warning: _Be sure not to place it in a directory whose path contains spaces_

### Step 6: Building an Extension

```java
//Save it as SimpleMaths.java
package com.makeroid; //package of the extension will be "com.makeroid.SimpleMaths"

//Only these imports are required to interact with Makeroid
import com.google.appinventor.components.annotations.*;
import com.google.appinventor.components.runtime.*;
import com.google.appinventor.components.common.*;

import android.content.Context; //You must add this

@DesignerComponent(
    version = 1, //Update version here, You must do for each new release to upgrade your extension
    description = "Simple Maths extension created by you",
    category = ComponentCategory.EXTENSION,
    nonVisible = true,
    iconName = "images/extension.png") //Change your extension's icon from here
@SimpleObject(external = true)

public class SimpleMaths extends AndroidNonvisibleComponent implements Component {
    private ComponentContainer container;
    private Context context;

    public SimpleExtension(ComponentContainer container) {
        super(container.$form());
        this.container = container;
        context = (Context) container.$context();
    }

    @SimpleFunction(description = "Simple addition of two numbers")
public double Add(double a, double b) {
    return a+b;
}

    @SimpleFunction(description = "Simple subtraction of two numbers")
public double Subtract(double a, double b) {
    return a-b;
}
}
```

* Download the file and move it to `appinventor-sources/appinventor/components/src/com/makeroid/`

* Go back to the `appinventor` folder.

* Open Command Prompt on that directory.

* Type `ant extensions` and click on enter.

#### _Wait for the extension to build..._

If it says: `BUILD SUCCESSFUL`, then you just created an extension :tada:  
But if it says: `BUILD FAILED`, then you did something wrong and have to look over again.

### Step 6: Sharing Extensions

Your extension file \(.aix file\) should appear in the directory:

**`appinventor-sources/appinventor/components/build/extensions`**

Now, you can easily share the aix files with anyone and can import it into Makeroid seemlessly.

---

##### For more information about extensions, read [here](http://ai2.appinventor.mit.edu/reference/other/extensions.html)

---

##### Keep making more and more and more extensions and help our community to build the best app.

#### [Share your extensions](https://community.makeroid.io/c/extensions) with our community and become an "[Extension Developer](https://community.makeroid.io/badges/102/extension-developer)".

---

If you want more help, feel free to ask us on [Makeroid Community](https://community.makeroid.io).

