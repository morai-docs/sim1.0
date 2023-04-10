# Sensor Settings
This section describes how to place each sensor provided by the simulator on the aircraft and set the sensor parameters to obtain sensor data.

---

## Sensor Placement

Place the sensors on the aircraft in the order below.

1) Click **∨** on the right side of the sensor icon in the menu at the top left as shown below.
   
<img src="../../img/ug-sensor-place.png" style="width: 500px; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

2) When you select a sensor to be placed in the popped-up sensor list, the following **Sensor Settings** window appears on the right. 
<br>

Ex) When selecting **Camera**
<img src="../../img/ug-sensor-setting1.png" style="width: auto; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

<img src="../../img/ug-sensor-setting.png" style="width: auto; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

3) When you click the mouse on the position of the aircraft where you want to place the sensor, the corresponding sensor item is created in **Sensor Settings**.
<Br>

Ex) When placing **Camera**
<img src="../../img/ug-sensor-setting-camera.png" style="width: 500px; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

### Adding sensors or placing different types of sensors
The method of adding the same type of sensor or placing a different type of sensor is the same as the sensor placement method **1) to 3)** above.

### Deleting placed sensors
In **Sensor Settings** on the right, click **...** of the sensor item you want to delete and click **Delete**.

Ex) When deleting **Camera**
<img src="../../img/ug-sensor-setting-delete2.png" style="width: 500px; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

<div markdown="span" class="bs-callout bs-callout-success">
✅ <span class = "suc-calloutTitle"> TIPS </span> <br>
The method for deleting other types of sensors is the same as above.
</div>

## Sensor Parameter Setting
In the sensor parameter setting, the parameters for the location coordinates (x, y, z) and posture (rotation angle of roll, pitch, and yaw) of the placed sensor and the specialized functions supported by each sensor model are set. <br>
When you click the created sensor item name (eg. **Camera-0**), the parameter setting window for the corresponding sensor appears as shown below.

Ex) Parameter setting window for **Camera**
<img src="../../img/ug-sensor-setting-camera2.png" style="width: 500px; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

### Location Coordinates
The location coordinates of all sensors provided by the simulator are set based on the aircraft coordinate system below.

<img src="../../img/ug-sensor-location.png" style="width: 500px; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

### Lens Distortion of Camera
The Lens Distortion effect reproduces the appearance of a real camera lens by distorting the final rendered image. <br>
The simulator's camera sensor model provides Lens Distortion as shown below.

<img src="../../img/sensor-lensdistortion.png" style="width: 500px; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

The setting parameter for lens distortion is as follows:

- K1, K2, K3: parameters related to radial distortion, simulating the phenomenon of radial distortion by the refractive index of a convex lens
- P1, P2: Parameter for making sensor attachment errors that occur during the camera assembly process

### Gaussian Noise of GNSS
The simulator's GPS sensor model supports Gaussian Noise as shown below.

<img src="../../img/sensor-gaussian.png" style="width: 500px; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

The value of Gaussian Noise is adjusted by entering **Mean(m)** and **Stdev(%)** values.

### Network Settings
The network of the sensor model provided by the simulator only sets UDP communication as shown below.

<img src="../../img/sensor-networksetting.png" style="width: 500px; height: auto;" alt="sensor" title="Click to Enlage" onclick="window.open(this.src)">

<div markdown="span" class="bs-callout bs-callout-success">
✅ <span class = "suc-calloutTitle"> TIPS </span> <br>
For information on how to set up a sensor network, see the <a href="../network/#sending-sensor-messages">Sending Sensor Messages</a> section.</div>