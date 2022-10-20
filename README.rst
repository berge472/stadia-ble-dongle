stadia-ble-dongle
====================

This project contains the source code for firmware to convert a USB HID device to a BLE HID device. The main purpose is to allow wireless use of stadia controllers. 

The initial proof of concept will target the `TinyS3 ESP32-S3 development board <https://www.amazon.com/gp/product/B09X259SDP>`_ , If that goes well, I will spin a custom PCB with a smaller (and hopefully more practical) form factor.



Building 
========

This project contains a devcontainer configuration. If you have docker installed, you dont need to worry about setting up the ESP32 development environment.

1. Install VS Code and the 'Remote Containers' extension
2. click the green remote button in the bottom left corner and select 'Reopen in Container'
3. open a terminal in vs code (ctrl+`) 

.. code:: bash 

    make 


Flashing
========