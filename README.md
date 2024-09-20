# Upgrade-to-another-smart-garage-door-opener

All smart garage door openers with remote controls on the market only work when the garage motor system is in standby mode.


I recently noticed that my garage door opener consumes more than 20W of power in standby mode.
I have now made the following modules. It should be operated by using a push button or a 433Mhz remote control or with the Home Assistant.

Every time you press the button to open or close the garage door, it works as follows:

1. Relay-1 operated for approx. 25s (this value can be set by using a slider in the Home Assistant) and connected the garage door system to the 220V supply.
2. Relay-2 turn on for 2s and then turn off. It will trigger the garage door opener for opening or closing.
3. Then after the specified time for e.g. 25s, everything is switched off until the next action.

**Components:**

  * nodemcu v3
  * 2-Channel Signal Relay Module
  * RF Module Receiver
  * 2 Wire Magnetic Reed Switch (Reed switches are used to monitor the opening and closing of the door)

![This is wiring diagram.](https://www.forgani.com/wp-content/2024/09/garage_4.jpg)

> [!NOTE]
> For more information: [Upgrade to another smart garage door opener](https://www.forgani.com/electronics-projects/8214-2/)

