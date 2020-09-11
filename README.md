# CSP_ARDUINO (Cubesat Space Protocol)

Cubesat Space Protocol (CSP) is a small protocol stack written in C. CSP is designed to ease communication between distributed embedded systems in smaller networks, such as Cubesats.

## Installation

Some stuff needed to the instalation

```bash
sudo apt-get update
sudo apt_get install gcc
sudo apt_get install python3
sudo apt-get install python-is-python3
sudo apt-get install libsocketcan-dev
sudo apt-get install -y libzmq3-dev
```

1.- Download the CSP_ARDUINO.zip

2.- Go to the Downloads folder, and unzip the CSP_ARDUINO.zip 

3.- Copy the "CSP_ARDUINO" folder to the Arduino folder, with the path arduino/hardware/arduino/avr/libraries
You can use the following command:

```bash
cp CSP_ARDUINO/ /home/user/arduino-1.8.13/hardware/arduino/avr/libraries
```

##### Note: The arduino folder could change with the Arduino version installed.

After this, you can import the csp.h library in your Arduino file.

## Compile

```bash
gcc prueba.c -o prueba -I include/ -I build/include/  build/libcsp.so build/libcsp.a -pthread
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

# Original Project

[CSP_LIBRARY](https://github.com/libcsp/libcsp)

Configure the Original Library

#### Configure FreeRTOS

```bash
./waf configure --install-csp --jobs=1 -o build_freertos -p --enable-rdp --enable-crc32 --enable-can-socketcan --enable-examples --with-os=freertos
```

#### Configure Linux(Posix)

```bash
./examples/buildall.py
```


