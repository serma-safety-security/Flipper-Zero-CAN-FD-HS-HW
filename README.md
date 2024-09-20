
# Flipper Zero CAN HS/FD Adapter

<div align="center">
  <img src="/Pictures/Banner.png" alt="Wiring diagram">
</div>


## Description: 

This project aims to develop a CAN (Controller Area Network) adapter for the Flipper Zero, allowing users to connect devices with a CAN interfaces in particular automotive ECU's.


## Firmware Development:

* The CAN adapter application firmware is developed in C++ using the Flipper Zero's Xtreme-Firmware SDK.
* The application firmware must runs on the Flipper Zero, which communicates with the CAN adapter through its SPI interface.

* Firmware features:
	- [x] CAN HS Communication
	- [] CAN FD Communication (partially)
    - [x] Device detection and configuration
	- [x] Error handling and debugging tools

* The CAN adapter is fully compatible with Linux SocketCAN enabling the usage of can-utils tooling for receiving and sending CAN messages. 

[See Software development folder for more information](https://example.com/redirect) 

## Hardware Development:

* The CAN adapter board is designed using KiCad 7.x
* The PCB layout includes:
	+ Microchip MCP2518FD CAN transceiver chip
	+ TJ1051i CAN driver with galvanic isolation up to 4kV 
	+ Screwless CAN connector for easy plug-in
	+ TX/RX CAN activity LEDs for easy debugging

[See Hardware development folder for more information](https://example.com/redirect)

## Getting Started:
* Download and install the CAN adapter application
* Launch the application and connect your Flipper Zero into your PC
* Find the appropriate COM port
* Setup the Flipper USB-CAN as a SocketCAN interface
```sh
sudo modprobe can$ sudo modprobe can-raw$ sudo modprobe slcan
sudo slcan_attach -f -s6 -o “<COM Port> (e.g. :/dev/ttyACM0)”
sudo slcand“<COM Port> (e.g :/dev/ttyACM0)” can0
sudo ifconfig can0 up
```

**Connection:**

![Wiring diagram](/Pictures/Connection.png)]
**Branches:**

* `main`: The main branch, where stable code is kept. This is the default branch that new users will see when they clone the repository.
* `dev`: The development branch, where experimental or feature-in-progress code lives. This allows for concurrent development and testing without affecting the stability of the main branch.

## Contributing:

* Before contributing, please create a new issue to propose your changes.
* Fork this repository to create a copy of the original.
* Create a new branch from `dev` (e.g., `feature/my-new-firmware`) for your feature or fix.
* Make your changes and commit them with descriptive commit messages.
* Push your branch to your forked repository.
* Open a pull request against the original `dev` branch.

## Testing:

TODO 

## License:

This project is licensed under the TODO. See `LICENSE` file for details.

# Acknowledgments:

* Special thanks to Kévin for the SW dev and Morike for the HW dev !  

