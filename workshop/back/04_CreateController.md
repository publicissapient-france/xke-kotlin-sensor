# Create a REST Controller

Let's go for the main part !

We need to create a RestController in order to collect data from sensors.

You can see an example of the input on [Apiary](http://docs.mnantern.apiary.io/#reference/0/sensor-data-collection/push-data):

```json
[
  {
    "smartphoneId": "42fc24f5-2391-4707-ab60-0975464bdc97",
    "type": "BRIGHTNESS",
    "eventTime": "2016-02-12T17:31:38Z",
    "value": "37"
  },
  {
    "smartphoneId": "42fc24f5-2391-4707-ab60-0975464bdc97",
    "type": "ACCELEROMETER",
    "eventTime": "2016-02-12T17:31:38Z",
    "value": "-1.80;4.72;8.27"
  }
]
```

You need to write on Standard output the following elements:

```
<x> elements in POST /data
<details of elt 1>
<details of elt 2>
```

For example:

```
2 elements in POST /data:
Data(smartphoneId=f98e9b49-8911-4e87-87f8-723588c2b09e, type=BRIGHTNESS, eventTime=2016-03-22T06:42:06Z, value=18.0)
Data(smartphoneId=f98e9b49-8911-4e87-87f8-723588c2b09e, type=ACCELEROMETER, eventTime=2016-03-22T06:42:06Z, value=-0.19613299;0.1176798;9.80665)
```

If you want to try your controller you can download the [Android application](https://github.com/mNantern/formation-cassandra/releases/download/AppMobile/cassandra_iot_5.apk)

Previous: [Project Creation](03_AddDataClass.md)

Next: [Spring Boot Configuration](05_Solution.md)

:horse:
