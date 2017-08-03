In this tutorial I am going to teach you how to create extensions for Makeroid.

### Tools you will need:

* [ ] [App Inventor Sources ](https://github.com/mit-cml/appinventor-sources)
* [ ] [Java JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
* [ ] [Apache Ant](http://ant.apache.org/bindownload.cgi)
* [ ] Java IDE/Text Editor \(Eclipse, NetBeans, IntelliJ IDEA, [Notepad++](https://notepad-plus-plus.org) are recommended\)
* [ ] ~~Git Bash~~

> Install everything listed above and let's get started!

### Step 1: Download and Install Java JDK

**Step 1: Download and Install Java JDK**

* Install Java JDK
* Set the Environmental Variables:

  * **Set**
    "
    `JAVA_HOME`
    " to your install Java install path. Example: "
    `C:/Java/jdk1.8.0_31`
    "
  * **Edit**  
    "  
    `PATH`  
    " and add those:

    `%JAVA_HOME%/bin`

    `%JAVA_HOME%/jre/bin`

  * **Set**  
    "  
    `CLASSPATH`  
    " to "  
    `%JAVA_HOME%/lib/dt.jar;%JAVA_HOME%/lib/tools.jar`  
    "

**Step 2: Download and Install Apache Ant**

Download Apache Ant 1.10.1

* Unzip the folder and move it to a place where it is safe
* Set the Environmental Variables:
  * **Set**
    "
    `ANT_HOME`
    " to the Folder where ant is. Example: "
    `C:/Ant/apache-ant-1.10.1`
    "
  * **Edit**
    "
    `Path`
    " and add "
    `Folder where ant is+ \bin`
    ". Example: "
    `C:/Ant/apache-ant-1.10.1\bin`
    "
  * **Edit**
    "
    `ClassPath`
    " and add "
    `Folder where ant is+ \lib`
    ". Example: "
    `C:/Ant/apache-ant-1.10.1\lib`
    "

**Step 3: Download and Install Git Bash**

* Download and Install Git Bash

**Step 4: Download AppInventor Sources**

* Download appinventor-sources
* Unzip the folder and move it to a place where it is safe

**Step 5: Testing if it works**

* Go to your appinventor-sources folder and open the
  `appinventor`
  folder
* Right click in the folder and select "
  `Git Bash Here`
  "
* Type "
  `ant`
  " and click on enter

If says: "`BUILD SUCCESSFUL`", then you can go to Step 6  
If says: "`BUILD FAILED`", then you did something wrong or missed a step

**Step 6: Building an Extension**

[SimpleExtension.java2](https://community.makeroid.tk/uploads/default/original/1X/96d886facb10457bf2eb9c36e00947987a2fa25f.java)\(2.8 KB\)

* Download the file and move it to "  
  `appinventor-sources/appinventor/components/src/com/sanderjochems/`  
  "

  **Note:**  
  _If you want a other package name, then you need to put the SimpleExtensions.java in a other folder and update the package name in the file_

* Go back to the "  
  `appinventor`  
  " folder

* Right click in the folder and select "
  `Git Bash Here`
  "
* Type "
  `ant extensions`
  " and click on enter

If says: "`BUILD SUCCESSFUL`", then you can create Extensions :tada:  
If says: "`BUILD FAILED`", then you did something wrong

