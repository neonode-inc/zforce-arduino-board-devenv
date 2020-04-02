# zforce-arduino-board-devenv

## Hardware requirement
This setup environment is intended to work with the Neonode Prototyping Board (later referred to as the board, or NPB). The board is an Arduino-compatible microcontroller board, based on the [SAMD21](https://www.microchip.com/wwwproducts/en/ATSAMD21E18) MCU. You can connect your Neonode Touch Sensor Module directly to the board through the mounted sensor port with all 8 connector pads exposed to the board.

For further details about the connector pads on the Touch Sensor Module, please refer to [Neonode support page](https://support.neonode.com/docs/display/AIRTSUsersGuide/Electrical+Integration). NPB is only intended for development and prototyping, meaning, it is not created to withstand challenging environments or demanding use-cases.

NPB can be configured using an Arduino development environment, for example the Arduino IDE. For easier configuration and implementation, include our [Arduino Library](https://github.com/neonode-inc/zforce-arduino) to your Touch Sensor Module project. 

## Set-up Guide in Arduino IDE

Download and Select Board

1. Go to File>>Preferences

2. in Preferences, navigate to Additional Boards Manager URLs and include the following URL:
`https://raw.githubusercontent.com/neonode-inc/zforce-arduino-board-devenv/master/package_neonode_index.json`
    > If you have multiple URLs in your Board Manager, you can separate each link with a comma (,) or press the pop-up icon and paste the URL on a new row.

3. Press OK.

4. Now, go to Tools>>Boards>>Boards Manager, and type "Neonode Prototyping Board" in the search field.

5. On Neonode Prototyping Board, Press Install.

6. When the installation is complete, Select the board in Arduino IDE by going to Tools>>Board>>Neonode Prototyping Board

7. Select AVRISP mrkII as Programmer. Go to Tools >> Programmer >> AVRISP mrkII.
    > Alternatively, you can select USBtinyISP as your programmer.

8. Include the zForce Library. Refer to our [Arduino Library](https://github.com/neonode-inc/zforce-arduino) for easier communication with the Neonode Touch Sensor Module.
