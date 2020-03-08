# LG-Climate-component-for-Home-Assistant
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
