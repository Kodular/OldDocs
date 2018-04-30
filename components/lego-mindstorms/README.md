---
description: >-
  These components provide control of LEGO® MINDSTORMS® NXT robots using
  Bluetooth.
---

# LEGO Mindstorms

LEGO and MINDSTORMS are registered trademarks of the LEGO Group.

IMPORTANT : All of these components have a BluetoothClient property that must be set in the App Inventor designer \(in the browser\). The property cannot be set in the blocks editor. The property tells which BluetoothClient component to use for communication with the robot. You will need to explicitly add a BluetoothClient component to your project. If you have one robot, you should have one BluetoothClient component. If you are lucky enough to have two robots and you want to control both of them simultaneously from one application, you'll need two BluetoothClient components in your project. The BluetoothClient component is available from the "Not ready for prime time" section of the palette.

Here's a list of the initial steps you'll need to perform to use one or more of the NXT components:

Go to the Palette and click on "Not ready for prime time".  
Drag a BluetoothClient component and drop it on to the Viewer .  
The component will automatically be named BluetoothClient1 .  
In the Palette , click on "LEGO MINDSTORMS".  
Drag one of the components, for example NxtDirectCommands , and drop it on to the Viewer .  
In the Properties box , click on the area after BluetoothClient \(currently "None..."\).  
A box appears with a list of all the BluetoothClient components in your project.  
Click on BluetoothClient1 and click OK .  
If desired, add another component, for example NxtColorSensor , and repeat steps 6-8 to set its BluetoothClient property.

{% page-ref page="nxt-drive.md" %}

{% page-ref page="nxt-color-sensor.md" %}

{% page-ref page="nxt-light-sensor.md" %}

{% page-ref page="nxt-sound-sensor.md" %}

{% page-ref page="nxt-touch-sensor.md" %}

{% page-ref page="nxt-ultrasonic-sensor.md" %}

{% page-ref page="nxt-direct-commands.md" %}

{% page-ref page="ev3-motors.md" %}

{% page-ref page="ev3-color-sensor.md" %}

{% page-ref page="ev3-gyro-sensor.md" %}

{% page-ref page="ev3-touch-sensor.md" %}

{% page-ref page="ev3-sound.md" %}

{% page-ref page="ev3-ui.md" %}

{% page-ref page="ev3-commands.md" %}

