# Create Extensions

This tutorial will guide you to create extensions for Makeroid.

---

### Tools you will need:

* [App Inventor Sources ](https://github.com/mit-cml/appinventor-sources)
* [Java JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
* [Apache Ant](http://ant.apache.org/bindownload.cgi)
* Java IDE/Text Editor \([Eclipse](http://www.eclipse.org/downloads/eclipse-packages/), [NetBeans](https://netbeans.org/downloads/), [IntelliJ IDEA](https://www.jetbrains.com/idea/download/), [Notepad++](https://notepad-plus-plus.org) are recommended\)

> Download everything listed above and let's get started!

### Step 1: Setting up Java JDK

* Install JDK

  > :warning: _Be sure not to install it in a directory whose path contains spaces_

* Set the Environmental Variables:

  * Set** **`JAVA_HOME` to where you installed Java JDK. For example: `C:\Program Files\Java\jdk1.8.0_131`
  * Edit** **`PATH` and add those:

    `%JAVA_HOME%/bin`, `%JAVA_HOME%/jre/bin`, `C:\ProgramData\Oracle\Java\javapath`

### Step 2: Setting up Apache Ant

* Unzip the folder and move it to a place where it is safe. For example: `C:\apache-ant-1.10.1`

  > :warning: _Be sure not to place it in a directory whose path contains spaces_

* Set the Environmental Variables:

  * **Set **`ANT_HOME` to where you have the Ant folder placed. For example: `C:/Ant/apache-ant-1.10.1`
  * **Edit **`Path` and add `<Ant Directory>\bin` For example: `C:/Ant/apache-ant-1.10.1\bin`
  * **Edit **`ClassPath` and add `<Ant Directory>\bin` For example: `C:/Ant/apache-ant-1.10.1\lib`

### Step 4: App Inventor Sources

* Unzip the folder and move it to a place where it is safe

  > :warning: _Be sure not to place it in a directory whose path contains spaces_

### Step 5: Checking Installation

To check whether you have everything installed correctly, just open a Command Prompt and check the following:

* **Check Java:** Execute `java -version`

```
  C:\Users\Pavitra>java -version
  java version "1.8.0_131"
  Java(TM) SE Runtime Environment (build 1.8.0_131-b11)
  Java HotSpot(TM) 64-Bit Server VM (build 25.131-b11, mixed mode)
```

* **Check Ant**: Execute `ant -version`

```
  C:\Users\Pavitra>ant -version
  Apache Ant(TM) version 1.10.1 compiled on February 2 2017
```

### Step 6: Building an Extension

> [SimpleExtension.java](https://community.makeroid.tk/uploads/default/original/1X/96d886facb10457bf2eb9c36e00947987a2fa25f.java) \(2.8 KB\)

* Download the file and move it to `appinventor-sources/appinventor/components/src/com/sanderjochems/`

  > **Note:**  
  > _If you want a other package name, then you need to put the SimpleExtensions.java in a other folder and update the package name in the file_

* Go back to the `appinventor` folder.

* Open Command Prompt on that directory.

* Type `ant extensions` and click on enter.

_**Wait for the extension to build...**_

If it says: `BUILD SUCCESSFUL`, then you just created an extension :tada:  
But if it says: `BUILD FAILED`, then you did something wrong and have to look over again.

---

#### Keep making more and more and more extensions and help our community to build the best app.

#### [Share your extensions](https://community.makeroid.tk/c/extensions) with our community and become an "[Extension Developer](https://community.makeroid.tk/badges/102/extension-developer)".

---

If you want more help, feel free to ask us on [Makeroid Community](https://community.makeroid.tk).

