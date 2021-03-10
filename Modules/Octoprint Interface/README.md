# Octoprint with Raspberry Pi 4.0

Here as mentioned in the introduction Octoprint will be running on the raspberry pi. Here the raspberry pi will be connected to the Teensy via serial and a 15" touch screen will be connected to the Raspberry. The screen used will be this: [Link](https://www.beetronics.dk/15-tommer-touchskaerm-metal-4-3). The reason this HMI is used is because the ease of use that octoprint offers and future expansion of functionality is easy.

#### Camera in octoprint

Here a Sony QX1 will be mounted on the printer to monitor the printing process. The QX1 already outputs a mjpeg stream over its own network. So here the raspberry pi will be connected to the QX1's network. and input the stream into octoprint. In the future this functionality will be expanded to sending trigger commands to the QX1 to take pictures so octolapse can be integrated. Here a problem arises if the raspberry pi is to be connected to wifi and controlled remotely. To solve this problem either a WiFi dongle will be connected or the ethernet port on the raspberry will be used. A power adapter will here be used to power the qx1 constantly. This power adapter can be seen here: [Link](https://www.subtel.dk/index.php?cl=details&offerId=3978956963&lang=6&anid=915664&cnid=192d2e4a1f71bd07ce1a5f9bbb185e09&campaign=dk-pla/Netzteil/915664&gclid=Cj0KCQiAs5eCBhCBARIsAEhk4r6M4nEBqRl9llAmq8cqiiVEmtkUiZZ6ZFrAzY_FEcEVpPGQpeQw50saAnzREALw_wcB)

##### Camera commands so far to get live-view

For saving the liveview this command have been used on MacOS for now:

```bash
ffmpeg -i http://192.168.122.1:8080/liveview/liveviewstream -vcodec flv -qscale 1 -an output.flv
```



### Bill of Materials

| Name                   | Quantity |                             Link                             | Price (DKK) |
| :--------------------- | :------: | :----------------------------------------------------------: | :---------: |
| ILCE-QX1 Power adapter |    1     | [Link](https://www.subtel.dk/index.php?cl=details&offerId=3978956963&lang=6&anid=915664&cnid=192d2e4a1f71bd07ce1a5f9bbb185e09&campaign=dk-pla/Netzteil/915664&gclid=Cj0KCQiAs5eCBhCBARIsAEhk4r6M4nEBqRl9llAmq8cqiiVEmtkUiZZ6ZFrAzY_FEcEVpPGQpeQw50saAnzREALw_wcB) |     259     |
| 15" Touch screen       |    1     | [Link](https://www.beetronics.dk/15-tommer-touchskaerm-metal-4-3) |    2699     |

