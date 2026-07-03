# LIXIL shutter BLE macros for Nature Remo

Nature Remo device-extension macros for LIXIL shutters that expose the following BLE endpoint:

- Service UUID: `2141e110-213a-11e6-b67b-9e71128cae77`
- Notify characteristic UUID: `2141e111-213a-11e6-b67b-9e71128cae77`
- Write characteristic UUID: `2141e112-213a-11e6-b67b-9e71128cae77`

The command is written to `2141e112...` using `WRITE_COMMAND`, then the macro waits for a notification on `2141e111...`.

## Nature Remo macro URLs

- Open: https://github.com/yamatohagi/lixil-shutter-ble-macros/blob/main/lixil-shutter-open.xml
- Close: https://github.com/yamatohagi/lixil-shutter-ble-macros/blob/main/lixil-shutter-close.xml
- Stop: https://github.com/yamatohagi/lixil-shutter-ble-macros/blob/main/lixil-shutter-stop.xml

Before testing, disconnect My Window and other phones from the shutter.
