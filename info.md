## MQTT Share integration

Allow the sharing of entities between multiple instances of Home Assistant using MQTT. Primarily tested with binary_sensor, switch, light, and fan entities.

### Features

* Support binary_sensor, switch, light, and fan entities.
* Supports isy994_control events.
* Supports call_service events which means remote switch, light or fan can be controlled.
* It is important that entity_ids be unique across all Home Assistant instances.

### Usage

For the MQTT Share integration all you need to do is specify MQTT ```base_topic:``` and it will automatically pick all shared entities from the remote Home Assistant instance running MQTT Share Remote.

```yaml
mqtt_share:
  base_topic: hass_share
```
