# HAjudoRest

Example of rest sensors for HomeAssistant to get local Judo iSoft Safe+ data via the Connectivity module (https://judo.eu/en/products/connectivity-modul-wlan/)

## Background

This provides a basic example how to aquire data from a Judo iSoft Safe+ water softening system via the Judo Rest interface into HomeAssistant.
The communication is local via the connectivity module, it does not require any cloud/web service. I use the LAN connection of the module.

## Notes

The water consumption value waterQty should be the total consuption, and it includes the soft water waterQtySoft. When comparing the values with the offical water meter the monthly consumption of the meter seems to be roughly the waterQty + waterQtySoft. It also seems to be very senstive to opening the valve all they way on the softening system.

To test inital access curl can be used to get data via the API.

## Links

The API can be found at https://judo.eu/en/products/api/. Hint: switch the web site language to german to get the link to the API document.
