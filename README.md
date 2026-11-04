# Tasmota 16.0.0 lvgl-haspmota + Domoticz + BH1750 + GY-302


Build ESP32-D0WD, ambiente PlatformIO `tasmota32-lvgl`, sorgente Tasmota v16.0.0.

Modifica in `tasmota/include/tasmota_configurations_ESP32.h`, nel blocco `#ifdef FIRMWARE_LVGL` (riga 304):
- `#undef USE_DOMOTICZ` commentato
- aggiunto `#define USE_BH1750`

Compilazione: `pio run -e tasmota32-lvgl` (circa 10 minuti la prima volta).
Aggiornamento: OTA con `tasmota32-lvgl.bin`, non il factory.
+ GY-302
