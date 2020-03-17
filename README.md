# zforce-arduino-board-devenv

## Hardware requirement
This setup environment is inteded to work with the Neonode Prototyping Board (later refered as the baord, or NPB). The board is an Arduino-compatible microcontroller board, based on the [SAMD21](https://www.microchip.com/wwwproducts/en/ATSAMD21E18) MCU. You can connect your zForce AIR Touch Sensor directly to the board through the mounted sensor port with all 8 connector pads exposed to the board.

For further details about the connector pads on the zForce AIR sensor, please refer to [Neonode support page](https://support.neonode.com/docs/). NPB is only intended for development and prototyping, meaning, it is not created to withstand challenging environments or demanding use-cases.

NPB can be configured using an Arduino development environment, for example the Arduino IDE. For easier configuration and implementation, include our [Arduino Library](https://github.com/neonode-inc/zforce-arduino) to your zForce AIR Project. 

## Set-up Guide in Arduino IDE

Download and Select Board

1. Go to File>>Preferences

2. In Preferences, navigate to Additional Boards Manager URLs and include the following link: `https://raw.githubusercontent.com/neonode-inc/zforce-arduino-board-devenv/master/package_neonode_index.json`
    > If you have multiple URLs in your Board Manager, you can separate each link with a comma (,) or press the pop-up icon and paste the URL on a new row.

3. Press OK.

4. Go to Tools>>Boards>>Boards Manager, and type "Neonode" in the search field. 

5. On Neonode Boards, press Install. 

6. When the installation is complete, Select the new board by going to Tools>>Board>>Neonode Adapter

7. Select AVRISP mrkII as Programmer. Go to Tools>>Programmer>>AVRISP mrkII.
    > Alternatively, you can select USBtinyISP as your programmer.

8. Include the zForce AIR Library. Refer to our [Arduino Library](https://github.com/neonode-inc/zforce-arduino) for easier communication with the zForce AIR Touch Sensor.
