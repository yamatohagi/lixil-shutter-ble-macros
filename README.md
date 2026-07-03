# LIXIL shutter BLE macros for Nature Remo

Experimental Nature Remo device-extension macros for LIXIL shutters that expose the following BLE endpoint:

- Service UUID: `2141e110-213a-11e6-b67b-9e71128cae77`
- Characteristic UUID: `2141e111-213a-11e6-b67b-9e71128cae77`

## Primary macros

- Open: `lixil-shutter-open.xml` writes `0203` using `WRITE_REQUEST`
- Close: `lixil-shutter-close.xml` writes `0204` using `WRITE_REQUEST`
- Stop: `lixil-shutter-stop.xml` writes `0205` using `WRITE_REQUEST`

## Fallback macros

If the primary macros fail because the characteristic only accepts write-without-response:

- Open: `lixil-shutter-open-command.xml` writes `0203` using `WRITE_COMMAND`
- Close: `lixil-shutter-close-command.xml` writes `0204` using `WRITE_COMMAND`
- Stop: `lixil-shutter-stop-command.xml` writes `0205` using `WRITE_COMMAND`

Before testing, disconnect My Window and other phones from the shutter.

## GitHub URLs for Nature Remo

Primary `WRITE_REQUEST` URLs:

- Open: https://github.com/yamatohagi/lixil-shutter-ble-macros/blob/main/lixil-shutter-open.xml
- Close: https://github.com/yamatohagi/lixil-shutter-ble-macros/blob/main/lixil-shutter-close.xml
- Stop: https://github.com/yamatohagi/lixil-shutter-ble-macros/blob/main/lixil-shutter-stop.xml

Fallback `WRITE_COMMAND` URLs:

- Open: https://github.com/yamatohagi/lixil-shutter-ble-macros/blob/main/lixil-shutter-open-command.xml
- Close: https://github.com/yamatohagi/lixil-shutter-ble-macros/blob/main/lixil-shutter-close-command.xml
- Stop: https://github.com/yamatohagi/lixil-shutter-ble-macros/blob/main/lixil-shutter-stop-command.xml
