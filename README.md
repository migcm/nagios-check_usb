# nagios-check_usb

NRPE Plugin - Check if a USB is plug-in to a computer or server.

To use this plugin it's necessary to have 'lsusb' installed on the machine where this script will be executed.
The USB ID can be found by executing 'lsusb' on the command line. The TAG can be anything that allows you to remember what USB device it's (must not contain blanks or dashes).
The plugin will return CRITICAL status if one of the USB identifiers isn't found.

### Syntax:
    ```check_usb usbID[-TAG] [usbID[-TAG]]```


### Examples:

```check_usb 016e:0423```

```check_usb 016e:0423 03ab:2312```

```check_usb 016e:0423 03ab:2312 01cb:2116 31ab:2812```

```check_usb 016e:0423-Micro 03ab:2312-Webcam 31ab:2812```

