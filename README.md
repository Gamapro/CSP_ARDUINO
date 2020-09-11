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

Copy the "CSP_ARDUINO" folder to the Arduino folder, with the path arduino/hardware/arduino/avr/libraries

After this, you can import the csp.h library in your Arduino file.

## Compile

```bash
gcc prueba.c -o prueba -I include/ -I build/include/  build/libcsp.so build/libcsp.a -pthread
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Original Project

[CSP_LIBRARY](https://github.com/libcsp/libcsp)

