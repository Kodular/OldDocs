# LEGO Mindstorms

These components provide control of LEGO® MINDSTORMS® NXT robots using Bluetooth.

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

* [**NXT Drive**](nxt-drive.md)
* [**NXT Color Sensor**](nxt-color-sensor.md)
* [**NXT Light Sensor**](nxt-light-sensor.md)
* [**NXT Sound Sensor**](nxt-sound-sensor.md)
* [**NXT Touch Sensor**](nxt-touch-sensor.md)
* [**NXT Ultrasonic Sensor**](nxt-ultrasonic-sensor.md)
* [**NXT Direct Commands**](nxt-direct-commands.md)
* [**EV3 Motors**](ev3-motors.md)
* [**EV3 Color Sensor**](ev3-color-sensor.md)
* [**EV3 Gyro Sensor**](ev3-gyro-sensor.md)
* [**EV3 Touch Sensor**](ev3-touch-sensor.md)
* [**EV3 Ultrasonic Sensor**](ev3-ultrasonic-sensor.md)
* [**EV3 Sound**](ev3-sound.md)
* [**EV3 UI**](ev3-ui.md)
* [**EV3 Commands**](ev3-commands.md)

