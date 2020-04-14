# LG-Climate-component-for-Home-Assistant
Based on my Tasmota Irhvac Custom Component

Currently tested and woring in Home Assistant up to v.108.3

Copy lg_climate folder to your `config/custom_component` folder

Restart Home assistant

Add the Example configuration to your configuration.yaml

Change `command_topic`, `state_topic` and `name` to fit your needs.

Restart Home Assistant again

Ready

example configuration in configuration.yaml
``` yaml
climate:
  - platform: lg_climate
    name: LG Clima
    command_topic: "cmnd/kitchenMultisensor/irsend"
    state_topic: "tele/kitchenMultisensor/RESULT"
    temperature_sensor: sensor.kitchen_temperature
    away_temp: 24 #optional (can be removed) - default 24 int value
```
For more info about `state_topic`, please read: [Tasmota Irhvac Repository](https://github.com/hristo-atanasov/Tasmota-IRHVAC)
