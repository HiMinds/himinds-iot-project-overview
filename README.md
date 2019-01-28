# himinds-iot-project-overview
The HiMinds IoT project consists of several sub-projects. In each project, we explore different technologies and implement a product consisting of hardware, back-end and mobile app.

Most of our work is documented in our [tech blog](https://medium.com/himinds) at https://medium.com/himinds.

Currently, we have the following projects:

* Home Energy Monitor :bulb:, exploring power signature analysis
* Smart BLE button :radio_button:, push a button and something happens :smile:

## :house: Energy Monitor :bulb:

### Project description:
A basic home energy monitor will show you your current energy consumption. More advanced energy monitors can show devices that
are currently active by identifying their unique power signature. In this project, we will build an advanced energy monitor that processes the data in the cloud using machine learning algorithms.

### Hardware/Technology stack:
* [ESP32](https://www.espressif.com/en/products/hardware/socs)
* [Mongoose OS](https://mongoose-os.com/)
* [Google Cloud IoT Core](https://cloud.google.com/iot-core/)
* [Firebase](https://firebase.google.com/)
* [React Native](https://facebook.github.io/react-native/)
* [Expo.io](https://expo.io/)
* [NativeBase](https://nativebase.io/)

### Relevent repositories:
* [himinds-iot-project-mobile-home-energy-monitor-app](https://github.com/HiMinds/himinds-iot-project-mobile-home-energy-monitor-app), React Native app that visualizes the power consumption
* [ESP32 IoT client to connect to Google IoT Core](https://github.com/HiMinds/himinds-iot-project-embedded-esp32-mongoose-gcp-iot-client)
* [himinds-iot-project-cloud-gcp-cloud-functions](https://github.com/HiMinds/himinds-iot-project-cloud-gcp-cloud-functions) back-end for Google IoT core demo
* [Provision Google IoT core using terraform](https://github.com/HiMinds/himinds-iot-project-cloud-terraform-gcp-template)
* [ESP32 and Mongoose OS setup](https://github.com/HiMinds/himinds-iot-project-embedded-esp32-mongoose-os-vscode-setup)
* [ADC simulator, perfect sine wave](https://github.com/HiMinds/himinds-iot-project-embedded-pc-nodejs-mqtt-adc-simulator) generate a sine wave (control frequency, amplitude, offset etc.)

### To-Do:
- [X] ESP32 WiFi and cloud connectivity
- [X] Simulate ADC hardware, publish MQTT message 
- [ ] Design hardware, HW to interface current sensor, non-invasive current sensor etc.
- [ ] Design algorithm in Energy Monitor
- [ ] Create tool plot sine wave in real-time
- [ ] Define MQTT protocol

### Issues:
- [ ] No. 2933, ADC configuration on ESP32, [Sample 100 Hz sine wave with ADC1_CHANNEL_4 from JavaScript or C](https://forum.mongoose-os.com/discussion/2933/sample-100-hz-sine-wave-with-adc1-channel-4-from-javascript-or-c)

### Learning resources
* [Electricity monitoring](https://learn.openenergymonitor.org/electricity-monitoring/ac-power-theory/introduction)
* [Power signature analysis](https://resenv.media.mit.edu/classarchive/MAS961/readings/PowerSignatureAnalysis.pdf)
* [Power Load Event Detection and Classification Based on Edge Symbol Analysis and Support Vector Machine](https://www.hindawi.com/journals/acisc/2012/742461/)

### Inspiration:
We are inspired by these cool companies:

* [wattcost](https://www.wattcost.com/)
* [WATTY](https://watty.io/)
* [sense](https://sense.com/)
* [Neurio](https://www.neur.io/)
* [Curb](https://energycurb.com/)
* [smappee](https://www.smappee.com/be_en/our-technology)

## Smart BLE button :radio_button:

### Project description:
We love the idea that only your imagination can limit what will happen when you push a button. In this project, we want to explore the challenges of building a push button that is if This Then That ready (IFTTT).

### Hardware/Technology stack:
* [Puck.js](https://www.puck-js.com/)
* [Raspberry Pi](https://www.raspberrypi.org/)
* [Mender](https://mender.io/)
* [Google Cloud IoT Core](https://cloud.google.com/iot-core/)
* [Firebase](https://firebase.google.com/)
* [React Native](https://facebook.github.io/react-native/)
* [Expo](https://expo.io/)
* [NativeBase](https://nativebase.io/)

### Relevent repositories:
* [BLE Pushbutton](https://github.com/HiMinds/himinds-iot-project-embedded-sensor-pushbutton-ble) for PuckJS
* [BLE to Google IoT core](https://github.com/HiMinds/himinds-iot-project-embedded-raspberrypi-nodejs-smart-ble-button) application for NodeJS running on Raspberry Pi

### To-Do:
- [x] Simple BLE pushbutton implementation using GAP profile
- [x] Write BLE application for NodeJS running on Raspberry Pi
- [x] Raspberry Pi with cloud connectivity
- [ ] OTA, Yocto, Mender and Raspberry Pi
- [ ] Wireframing/mock-up App
- [ ] Switch to using GATT profile


### Inspiration:
We are inspired by these cool companies:

* [Qmote S](https://qblinks.com/)
* [niu](https://www.myniu.fr/en/)
* [POP Smart Button](https://www.logitech.com/en-us/product/pop-smart-button)
* [flic](https://flic.io/)
