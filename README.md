# ESPHome_TPMS

While a lot of research has been done on BLE TPMS sensors, very few ESPHome templates exists for them. It seems to me that there are slight variations of these sensors too, with different formats. This is my work on one of these formats.

The sensors I have starts with the MAC address "AC:15:85" and shows up with the name "BR" with a BLE scanning app. They Advertise a service as "0x27a5" with an empty payload. The manufacturer id and manufacturer data seems to contain the actual data we're interested in

We can get this data with the following snippet
```


```

Given the example 0x1E00 1A:00:95:A4:79, where:

`1E` is the battery voltage (3.0v)

`1A` is the temperature in degree celcius (26 degree)

`00:95` is the pressure in kpa (149 kpa)


# TPMS firmware in action
![Sensors](assets/sensors.png)
