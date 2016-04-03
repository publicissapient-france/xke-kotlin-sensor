# Get sensor value

Choose a [Sensor Type](http://developer.android.com/guide/topics/sensors/sensors_overview.html)

*Tips*: choose `TYPE_ACCELEROMETER` or `TYPE_LIGHT`.

You have to **listen** to sensor event to be able to get **notified** when sensor value changes.

To do so you have to **extend** [SensorEventListener](http://developer.android.com/reference/android/hardware/SensorEventListener.html)

And **implement** method [onSensorChanged](http://developer.android.com/reference/android/hardware/SensorEventListener.html#onSensorChanged(android.hardware.SensorEvent))

In this methods [update](http://developer.android.com/reference/android/widget/TextView.html#setText(java.lang.CharSequence)) `TextView` to display sensor value.

Good job! Now your application display sensor value when you get an update from the manager.

Next step consists to [subscribe to sensor](06_SubscribeToSensor.md).
