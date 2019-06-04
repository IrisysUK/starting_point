# Welcome to the Irisys github repos.

Here you will be able to find code samples and guidance on how to communicate with our devices.


## Data collection

### Vector

There are multiple ways of collecting data from Vector devices depending on your data requirements.

#### Logged data

Logged data is data that is stored on the Vector device to be retrieved at a later time. The minimum granularity of this data is 1 minute. You have the following options for collecting this data.

* Connect the devices to an Estate Manager instance and use the Estate Manager REST APIs to gather the data (sample: https://github.com/IrisysUK/emrestapi) If you have other Irisys devices e.g Gazelles then this is the recommended route as the Estate Manager REST API supports all device types.

* Configure the device to send data via HTTP POST (sample: https://github.com/IrisysUK/vectorhttppost) This will allow the device to send data to a location of your choosing when the data is logged to the device.

* Direct to device REST API (Sample: https://github.com/IrisysUK/vectorrestapi) This allows you to talk directly to a Vector device via a REST API to get access to the data.

#### Real-time data

Real-time data is timestamped information about what the device sees packaged up into sensible chunks of data. If you require data on sub 1 minute granularity then this is the best choice. You have the following options for collecting this data.

* MQTT Counts and Target X / Y positions (Sample: https://github.com/IrisysUK/mqtt-xy-demo) This allows you to get real-time count data along with information about the x / y position of any targets in the field of view of the device.


### Gazelle and 3000 series

To collect data from Irisys Gazelle and 3000 series devices we recommend you use Estate Manager and the relevant APIs. The samples for using the Estate Manager REST API can be found here: https://github.com/IrisysUK/emrestapi
