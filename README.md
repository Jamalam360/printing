# 3D Printing Files

Contains Orca Slicer profiles and a custom Marlin configuration for my CR10-V2.

## Marlin Changes

### Filament Runout Sensor

- Temporarily disabled.

### H2 V2S Extruder

_[Reference](https://cdn.shopify.com/s/files/1/1619/4791/files/4050000035-H2_500_user_manual.pdf?v=1679589018)_

- Set `DEFAULT_AXIS_STEPS_PER_UNIT` to `932` steps/mm for the extruder.

### Mesh Bed Leveling

- `PREHEAT_BEFORE_LEVELING` is enabled.

A new `CR10V2_MESH_BED_LEVELING` option is added. When enabled, the following settings are configured:

- `MESH_BED_LEVELING` is enabled.
- `RESTORE_LEVELING_AFTER_G28` is enabled.
- `LCD_BED_LEVELING` is enabled.
- `BABYSTEPPING` (_adv_) is enabled.

### SD Card Sorting

- `SDCARD_RATHERRECENTFIRST` (_adv_) is enabled to sort SD entries by most recently modified first.

### LCD Sound

- `SOUND_MENU_ITEM` (_adv_) is enabled.
- `SOUND_ON_DEFAULT` (_adv_) is disabled.
