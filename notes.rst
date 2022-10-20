Notes 
=====

Stadia controller enumeration on Windows 10 shows it as a composite device. One Interface is HID, and the other is a non-standard. The non standard only has 2 endpoints, a bulk-in and bulk-out. Most likely this is for firmware updates. 

.. code:: 
    
    [Port4]  :  USB Composite Device


    Is Port User Connectable:         yes
    Is Port Debug Capable:            no
    Companion Port Number:            4
    Companion Hub Symbolic Link Name: USB#VID_291A&PID_8392#MSFT30000000001#{f18a0e88-c30c-11d0-8815-00a0c906bed8}
    Protocols Supported:
    USB 1.1:                         yes
    USB 2.0:                         yes
    USB 3.0:                         no

    Device Power State:               PowerDeviceD0

        ---===>Device Information<===---
    English product name: "Stadia Controller rev. A"

    ConnectionStatus:                  
    Current Config Value:              0x01  -> Device Bus Speed: High (is not SuperSpeed or higher capable)
    Device Address:                    0x27
    Open Pipes:                           4

            ===>Device Descriptor<===
    bLength:                           0x12
    bDescriptorType:                   0x01
    bcdUSB:                          0x0201
    bDeviceClass:                      0xEF  -> This is a Multi-interface Function Code Device
    bDeviceSubClass:                   0x02  -> This is the Common Class Sub Class
    bDeviceProtocol:                   0x01  -> This is the Interface Association Descriptor protocol
    bMaxPacketSize0:                   0x40 = (64) Bytes
    idVendor:                        0x18D1 = Google Inc.
    idProduct:                       0x9400
    bcdDevice:                       0x0100
    iManufacturer:                     0x01
        English (United States)  "Google LLC"
    iProduct:                          0x02
        English (United States)  "Stadia Controller rev. A"
    iSerialNumber:                     0x03
        English (United States)  "99100YCAC28MLD"
    bNumConfigurations:                0x01

            ---===>Open Pipes<===---

            ===>Endpoint Descriptor<===
    bLength:                           0x07
    bDescriptorType:                   0x05
    bEndpointAddress:                  0x87  -> Direction: IN - EndpointID: 7
    bmAttributes:                      0x02  -> Bulk Transfer Type
    wMaxPacketSize:                  0x0200 = 0x200 max bytes
    bInterval:                         0x00

            ===>Endpoint Descriptor<===
    bLength:                           0x07
    bDescriptorType:                   0x05
    bEndpointAddress:                  0x07  -> Direction: OUT - EndpointID: 7
    bmAttributes:                      0x02  -> Bulk Transfer Type
    wMaxPacketSize:                  0x0200 = 0x200 max bytes
    bInterval:                         0x00

            ===>Endpoint Descriptor<===
    bLength:                           0x07
    bDescriptorType:                   0x05
    bEndpointAddress:                  0x83  -> Direction: IN - EndpointID: 3
    bmAttributes:                      0x03  -> Interrupt Transfer Type
    wMaxPacketSize:                  0x0040 = 1 transactions per microframe, 0x40 max bytes
    bInterval:                         0x06

            ===>Endpoint Descriptor<===
    bLength:                           0x07
    bDescriptorType:                   0x05
    bEndpointAddress:                  0x03  -> Direction: OUT - EndpointID: 3
    bmAttributes:                      0x03  -> Interrupt Transfer Type
    wMaxPacketSize:                  0x0040 = 1 transactions per microframe, 0x40 max bytes
    bInterval:                         0x06

        ---===>Full Configuration Descriptor<===---

            ===>Configuration Descriptor<===
    bLength:                           0x09
    bDescriptorType:                   0x02
    wTotalLength:                    0x0050  -> Validated
    bNumInterfaces:                    0x02
    bConfigurationValue:               0x01
    iConfiguration:                    0x00
    bmAttributes:                      0x80  -> Bus Powered
    MaxPower:                          0xFA = 500 mA

            ===>IAD Descriptor<===
    bLength:                           0x08
    bDescriptorType:                   0x0B
    bFirstInterface:                   0x00
    bInterfaceCount:                   0x01
    *!*ERROR:  bInterfaceCount must be greater than 1 
    bFunctionClass:                    0xFF  -> Interface Class Unknown to USBView
    bFunctionSubClass:                 0x00
    bFunctionProtocol:                 0x00
    iFunction:                         0x00

            ===>Interface Descriptor<===
    bLength:                           0x09
    bDescriptorType:                   0x04
    bInterfaceNumber:                  0x00
    bAlternateSetting:                 0x00
    bNumEndpoints:                     0x02
    bInterfaceClass:                   0xFF  -> Interface Class Unknown to USBView
    bInterfaceSubClass:                0x00
    bInterfaceProtocol:                0x00
    iInterface:                        0x00

            ===>Endpoint Descriptor<===
    bLength:                           0x07
    bDescriptorType:                   0x05
    bEndpointAddress:                  0x87  -> Direction: IN - EndpointID: 7
    bmAttributes:                      0x02  -> Bulk Transfer Type
    wMaxPacketSize:                  0x0200 = 0x200 max bytes
    bInterval:                         0x00

            ===>Endpoint Descriptor<===
    bLength:                           0x07
    bDescriptorType:                   0x05
    bEndpointAddress:                  0x07  -> Direction: OUT - EndpointID: 7
    bmAttributes:                      0x02  -> Bulk Transfer Type
    wMaxPacketSize:                  0x0200 = 0x200 max bytes
    bInterval:                         0x00

            ===>IAD Descriptor<===
    bLength:                           0x08
    bDescriptorType:                   0x0B
    bFirstInterface:                   0x01
    bInterfaceCount:                   0x01
    *!*ERROR:  bInterfaceCount must be greater than 1 
    bFunctionClass:                    0x03  -> HID Interface Class
    bFunctionSubClass:                 0x00
    bFunctionProtocol:                 0x00
    iFunction:                         0x00

            ===>Interface Descriptor<===
    bLength:                           0x09
    bDescriptorType:                   0x04
    bInterfaceNumber:                  0x01
    bAlternateSetting:                 0x00
    bNumEndpoints:                     0x02
    bInterfaceClass:                   0x03  -> HID Interface Class
    bInterfaceSubClass:                0x00
    bInterfaceProtocol:                0x00
    iInterface:                        0x00

            ===>HID Descriptor<===
    bLength:                           0x09
    bDescriptorType:                   0x21
    bcdHID:                          0x0111
    bCountryCode:                      0x00
    bNumDescriptors:                   0x01
    bDescriptorType:                   0x22 (Report Descriptor)
    wDescriptorLength:               0x00B6

            ===>Endpoint Descriptor<===
    bLength:                           0x07
    bDescriptorType:                   0x05
    bEndpointAddress:                  0x83  -> Direction: IN - EndpointID: 3
    bmAttributes:                      0x03  -> Interrupt Transfer Type
    wMaxPacketSize:                  0x0040 = 1 transactions per microframe, 0x40 max bytes
    bInterval:                         0x06

            ===>Endpoint Descriptor<===
    bLength:                           0x07
    bDescriptorType:                   0x05
    bEndpointAddress:                  0x03  -> Direction: OUT - EndpointID: 3
    bmAttributes:                      0x03  -> Interrupt Transfer Type
    wMaxPacketSize:                  0x0040 = 1 transactions per microframe, 0x40 max bytes
    bInterval:                         0x06

            ===>BOS Descriptor<===
    bLength:                           0x05
    bDescriptorType:                   0x0F
    wTotalLength:                      0x0039
    bNumDeviceCaps:                    0x02

            ===>Platform Capability Descriptor<===
    bLength:                           0x18
    bDescriptorType:                   0x10
    bDevCapabilityType:                0x05
    bReserved:                         0x00
    Platform Capability UUID:          3408B638-09A9-47A0-8BFD-A0768815B665
    00 01 01 00 

            ===>Platform Capability Descriptor<===
    bLength:                           0x1C
    bDescriptorType:                   0x10
    bDevCapabilityType:                0x05
    bReserved:                         0x00
    Platform Capability UUID:          D8DD60DF-4589-4CC7-9CD2-659D9E648A9F
    00 00 03 06 B2 00 02 00 
