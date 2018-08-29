# nagios-check_usb

Check if a USB is plug-in to a computer or server.

To use this plugin it's necessary to have 'lsusb' installed on the machine where this script will be executed.
The USB identifier can be found by executing 'lsusb' on the command line.
The plugin will return CRITICAL status if one of the USB identifiers isn't found.

### Syntax:
    ```check_usb USB-ID [USB-ID:]```


### Examples:
```check_usb 016e:0423```
```check_usb 016e:0423 03ab:2312```
```check_usb 016e:0423 03ab:2312 01cb:2116 31ab:2812```
