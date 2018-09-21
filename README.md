# himinds-iot-project-overview
The HiMinds IoT project consists of several sub-projects. In each project, we explore different technologies and implement a product consisting of hardware, back-end and mobile app.

Currently, we have the following projects:

* Home Energy Monitor :bulb:, exploring power signature analysis
* Smart BLE button :radio_button:, push a button and something happens :-)


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
* [Expo](https://expo.io/)
* [NativeBase](https://nativebase.io/)

### Relevent repositories:
* [ESP32 and Mongoose OS setup](https://github.com/HiMinds/himinds-iot-project-embedded-esp32-mongoose-os-vscode-setup)

### To-Do:
- [ ] Design hardware, HW to interface current sensor, non-invasive current sensor etc.
- [ ] Simulate hardware, generate a sine wave (control frequency, amplitude, offset etc.)
- [ ] Design algorithm in Energy Monitor
- [ ] Create tool plot sine wave in real-time
- [ ] Wireframing/mock-up App
- [ ] ESP32 WiFi and cloud connectivity
- [ ] Define MQTT protocol
- [ ] TBD


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
* [BLE Pushbutton](https://github.com/HiMinds/himinds-iot-project-embedded-sensor-pushbutton-ble)

### To-Do:
- [x] Simple BLE pushbutton implementation using GAP profile
- [ ] Switch to using GATT profile
- [ ] Write BLE application for NodeJS running on Raspberry Pi
- [ ] OTA, Yocto, Mender and Raspberry Pi
- [ ] Raspberry Pi with cloud connectivity
- [ ] Wireframing/mock-up App
- [ ] IFTTT integration


### Inspiration:
We are inspired by these cool companies:

* [Qmote S](https://qblinks.com/
* [niu](hhttps://www.myniu.fr/en/)
* [POP Smart Button](https://www.logitech.com/en-us/product/pop-smart-button)
* [flic](https://flic.io/)
