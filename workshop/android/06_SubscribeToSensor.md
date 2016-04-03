# Subscribe to sensor

In method [onCreate](http://developer.android.com/reference/android/app/Activity.html#onCreate(android.os.Bundle)) get a [SensorManager](http://developer.android.com/reference/android/hardware/SensorManager.html).

Register a listener for desired sensor.

Run the application.

If you have done all right you should see your `TextView` changing.

> Kotlin Tips
>
> You can use [delegate](https://kotlinlang.org/docs/reference/delegated-properties.html) to initialize your SensorManager

Let's [send data to HTTP API](07_SendValueToHttp.md)
