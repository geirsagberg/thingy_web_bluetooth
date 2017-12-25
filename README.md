<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [batteryLevelEnable](#batterylevelenable)
-   [buttonEnable](#buttonenable)
-   [colorEnable](#colorenable)
-   [colorSensorCalibrate](#colorsensorcalibrate)
-   [connect](#connect)
-   [constructor](#constructor)
-   [disconnect](#disconnect)
-   [eulerEnable](#eulerenable)
-   [externalPinControl](#externalpincontrol)
-   [externalPinsStatus](#externalpinsstatus)
-   [gasEnable](#gasenable)
-   [getAdvParams](#getadvparams)
-   [getBatteryLevel](#getbatterylevel)
-   [getCloudToken](#getcloudtoken)
-   [getConnParams](#getconnparams)
-   [getEddystoneUrl](#geteddystoneurl)
-   [getEnvironmentConfig](#getenvironmentconfig)
-   [getFirmwareVersion](#getfirmwareversion)
-   [getLedStatus](#getledstatus)
-   [getMotionConfig](#getmotionconfig)
-   [getMotionConfig](#getmotionconfig-1)
-   [getMtu](#getmtu)
-   [getName](#getname)
-   [gravityVectorEnable](#gravityvectorenable)
-   [headingEnable](#headingenable)
-   [humidityEnable](#humidityenable)
-   [ledBreathe](#ledbreathe)
-   [ledConstant](#ledconstant)
-   [ledOneShot](#ledoneshot)
-   [motionRawEnable](#motionrawenable)
-   [orientationEnable](#orientationenable)
-   [pressureEnable](#pressureenable)
-   [quaternionEnable](#quaternionenable)
-   [rotationMatrixEnable](#rotationmatrixenable)
-   [setAdvParams](#setadvparams)
-   [setCloudToken](#setcloudtoken)
-   [setColorInterval](#setcolorinterval)
-   [setConnInterval](#setconninterval)
-   [setConnSlaveLatency](#setconnslavelatency)
-   [setConnTimeout](#setconntimeout)
-   [setEddystoneUrl](#seteddystoneurl)
-   [setGasInterval](#setgasinterval)
-   [setHumidityInterval](#sethumidityinterval)
-   [setMagnetCompInterval](#setmagnetcompinterval)
-   [setMotionProcessFrequency](#setmotionprocessfrequency)
-   [setMtu](#setmtu)
-   [setName](#setname)
-   [setPressureInterval](#setpressureinterval)
-   [setStepCounterInterval](#setstepcounterinterval)
-   [setTemperatureCompInterval](#settemperaturecompinterval)
-   [setTemperatureInterval](#settemperatureinterval)
-   [setWakeOnMotion](#setwakeonmotion)
-   [stepEnable](#stepenable)
-   [tapEnable](#tapenable)
-   [temperatureEnable](#temperatureenable)

## batteryLevelEnable

Enables battery level notifications.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on battery level change. Will receive a battery level object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## buttonEnable

Enables button notifications from Thingy. The assigned event handler will be called when the button on the Thingy is pushed or released.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a button object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise with button state when resolved or a promise with an error on rejection.

## colorEnable

Enables color sensor notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a color sensor object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## colorSensorCalibrate

Configures color sensor LED calibration parameters.

**Parameters**

-   `red` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The red intensity, ranging from 0 to 255.
-   `green` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The green intensity, ranging from 0 to 255.
-   `blue` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The blue intensity, ranging from 0 to 255.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## connect

Connects to Thingy.
 The function stores all discovered services and characteristics to the Thingy object.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns an empty promise when resolved or a promise with error on rejection

## constructor

Thingy:52 Web Bluetooth API. <br> 
 BLE service details [here](https://nordicsemiconductor.github.io/Nordic-Thingy52-FW/documentation/firmware_architecture.html#fw_arch_ble_services)

**Parameters**

-   `options` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** Options object for Thingy (optional, default `{logEnabled:false}`)
    -   `options.logEnabled` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables logging of all BLE actions.

## disconnect

Method to disconnect from Thingy.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns an empty promise when resolved or a promise with error on rejection.

## eulerEnable

Enables Euler angle data notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive an Euler angle data object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## externalPinControl

Set an external pin to chosen state.

**Parameters**

-   `pin` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Determines which pin is set. Range 1 - 4.
-   `value` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Sets the value of the pin. 0 = OFF, 255 = ON.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## externalPinsStatus

Gets the current external pin settings from the Thingy device. Returns an object with pin status information.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns an external pin status object.

## gasEnable

Enables gas notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a gas object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## getAdvParams

Gets the current advertising parameters

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns an object with the advertising parameters when resolved or a promise with error on rejection.

## getBatteryLevel

Gets the battery level of Thingy.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns battery level in percentage when promise is resolved or an error if rejected.

## getCloudToken

Gets the configured cloud token.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns a string with the cloud token when resolved or a promise with error on rejection.

## getConnParams

Gets the current connection parameters.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns an object with the connection parameters when resolved or a promise with error on rejection.

## getEddystoneUrl

Gets the configured Eddystone URL

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([URL](https://developer.mozilla.org/en-US/docs/Web/API/URL/URL) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns a string with the URL when resolved or a promise with error on rejection.

## getEnvironmentConfig

Gets the current configuration of the Thingy environment module.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns an environment configuration object when promise resolves, or an error if rejected.

## getFirmwareVersion

Gets the current firmware version.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns a string with the firmware version or a promise with error on rejection.

## getLedStatus

Gets the current LED settings from the Thingy device. Returns an object with structure that depends on the settings.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)>** Returns a LED status object. The content and structure depends on the current mode.

## getMotionConfig

Motion service

## getMotionConfig

Gets the current configuration of the Thingy motion module.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns a motion configuration object when promise resolves, or an error if rejected.

## getMtu

Gets the current Maximal Transmission Unit (MTU)

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns the MTU when resolved or a promise with error on rejection.

## getName

Gets the name of the Thingy device.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;([string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) \| [Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error))>** Returns a string with the name when resolved or a promise with error on rejection.

## gravityVectorEnable

Enables gravity vector notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a heading object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## headingEnable

Enables heading notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a heading object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## humidityEnable

Enables humidity notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a humidity object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## ledBreathe

Sets the LED in "breathe" mode where the LED continuously pulses with the specified color, intensity and delay between pulses.

**Parameters**

-   `params` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** Options object for LED breathe mode
    -   `params.color` **([number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number) \| [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String))** The color code or color name. 1 = red, 2 = green, 3 = yellow, 4 = blue, 5 = purple, 6 = cyan, 7 = white.
    -   `params.intensity` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Intensity of LED pulses. Range from 0 to 100 [%].
    -   `params.delay` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Delay between pulses in milliseconds. Range from 50 ms to 10 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a resolved promise or an error in a rejected promise.

## ledConstant

Sets the LED in constant mode with the specified RGB color.

**Parameters**

-   `color` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** Color object with RGB values
    -   `color.red` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The value for red color in an RGB color. Ranges from 0 to 255.
    -   `color.green` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The value for green color in an RGB color. Ranges from 0 to 255.
    -   `color.blue` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The value for blue color in an RGB color. Ranges from 0 to 255.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a resolved promise or an error in a rejected promise.

## ledOneShot

Sets the LED in one-shot mode. One-shot mode will result in one single pulse of the LED.

**Parameters**

-   `params` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** Option object for LED in one-shot mode
    -   `params.color` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The color code. 1 = red, 2 = green, 3 = yellow, 4 = blue, 5 = purple, 6 = cyan, 7 = white.
    -   `params.intensity` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Intensity of LED pulses. Range from 0 to 100 [%].

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a resolved promise or an error in a rejected promise.

## motionRawEnable

Enables raw motion data notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a raw motion data object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## orientationEnable

Enables orientation detection notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a orientation detection object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## pressureEnable

Enables pressure notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a pressure object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## quaternionEnable

Enables quaternion notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a quaternion object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## rotationMatrixEnable

Enables rotation matrix notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive an rotation matrix object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## setAdvParams

Sets the advertising parameters

**Parameters**

-   `params` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** Object with key/value pairs 'interval' and 'timeout': <code>{interval: someInterval, timeout: someTimeout}</code>.
    -   `params.interval` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The advertising interval in milliseconds in the range of 20 ms to 5 000 ms.
    -   `params.timeout` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The advertising timeout in seconds in the range 1 s to 180 s.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise.

## setCloudToken

Sets the cloud token.

**Parameters**

-   `token` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** The cloud token to be stored.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise.

## setColorInterval

Sets the color sensor update interval.

**Parameters**

-   `interval` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Color sensor sampling interval in milliseconds. Must be in the range 200 ms to 60 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## setConnInterval

Sets the connection interval

**Parameters**

-   `params` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** Connection interval object: <code>{minInterval: someValue, maxInterval: someValue}</code>
    -   `params.minInterval` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The minimum connection interval in milliseconds. Must be >= 7.5 ms.
    -   `params.maxInterval` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The maximum connection interval in milliseconds. Must be &lt;= 4 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise.

## setConnSlaveLatency

Sets the connection slave latency

**Parameters**

-   `slaveLatency` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The desired slave latency in the range from 0 to 499 connection intervals.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)>** Returns a promise.

## setConnTimeout

Sets the connection supervision timeout
	<b>Note:</b> According to the Bluetooth Low Energy specification, the supervision timeout in milliseconds must be greater
 than (1 + slaveLatency) _ maxConnInterval _ 2, where maxConnInterval is also given in milliseconds.

**Parameters**

-   `timeout` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The desired connection supervision timeout in milliseconds and in the range of 100 ms to 32 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise.

## setEddystoneUrl

Sets the Eddystone URL
 It's recommeended to use URL shortener to stay within the limit of 14 characters long URL
 URL scheme prefix such as "https&#x3A;//" and "<https://www.>" do not count towards that limit,
 neither does expansion codes such as ".com/" and ".org".
 Full details in the Eddystone URL specification: <https://github.com/google/eddystone/tree/master/eddystone-url>

**Parameters**

-   `urlString`  
-   `url` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** The URL that should be broadcasted.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise.

## setGasInterval

Sets the gas sensor sampling interval.

**Parameters**

-   `interval` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The gas sensor update interval in seconds. Allowed values are 1, 10, and 60 seconds.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## setHumidityInterval

Sets the humidity measurement update interval.

**Parameters**

-   `interval` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Humidity sensor interval in milliseconds. Must be in the range 100 ms to 60 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## setMagnetCompInterval

Sets the magnetometer compensation interval.

**Parameters**

-   `interval` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Magnetometer compensation interval in milliseconds. Must be in the range 100 ms to 1 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## setMotionProcessFrequency

Sets motion processing unit update frequency.

**Parameters**

-   `frequency` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Motion processing frequency in Hz. The allowed range is 5 - 200 Hz.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## setMtu

Sets the current Maximal Transmission Unit (MTU)

**Parameters**

-   `params` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** MTU settings object: {mtuSize: value, peripheralRequest: value}, where peripheralRequest is optional. (optional, default `{peripheralRequest:false}`)
    -   `params.mtuSize` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The desired MTU size.
    -   `params.peripheralRequest` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Optional. Set to <code>true</code> if peripheral should send an MTU exchange request. Default is <code>false</code>;

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise.

## setName

Sets the name of the Thingy device.

**Parameters**

-   `name` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** The name that will be given to the Thingy.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise.

## setPressureInterval

Sets the pressure measurement update interval.

**Parameters**

-   `interval` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** The pressure sensor update interval in milliseconds. Must be in the range 50 ms to 60 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## setStepCounterInterval

Sets the step counter interval.

**Parameters**

-   `interval` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Step counter interval in milliseconds. Must be in the range 100 ms to 5 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## setTemperatureCompInterval

Sets the temperature compensation interval.

**Parameters**

-   `interval` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Temperature compensation interval in milliseconds. Must be in the range 100 ms to 5 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## setTemperatureInterval

Sets the temperature measurement update interval.

**Parameters**

-   `interval` **[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** Temperature sensor update interval in milliseconds. Must be in the range 100 ms to 60 000 ms.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## setWakeOnMotion

Sets wake-on-motion feature to enabled or disabled state.

**Parameters**

-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Set to True to enable or False to disable wake-on-motion feature.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection.

## stepEnable

Enables step counter notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a step counter object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## tapEnable

Enables tap detection notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a tap detection object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection

## temperatureEnable

Enables temperature notifications from Thingy. The assigned event handler will be called when notifications are received.

**Parameters**

-   `eventHandler` **[function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** The callback function that is triggered on notification. Will receive a temperature object as argument.
-   `enable` **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Enables notifications if true or disables them if set to false.

Returns **[Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)&lt;[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)>** Returns a promise when resolved or a promise with an error on rejection
