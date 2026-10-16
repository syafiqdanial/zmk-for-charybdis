# Syafiq Nano35 test build

Base: Vzhao-L/zmk-for-charybdis branch `charybdis-Nano35` at c82021984e997af65ef6d96083bf61dc79708003.

Keymap: copied from Syafiq's existing 35-position Nano firmware source (`syafiqdanial/ZMK_Charybdis_Nano`, local source aed9249). All 35-key bindings, combos, layers, and macros are unchanged. Removed only its reference to `five_column_transform`, a label from the old shield that does not exist in the maker's shield; the maker's 35-position transform remains in effect. The PMW3610 scroll layer selector is changed from the maker's layer 1 to keymap layer 5. Matrix GPIOs and sensor wiring are otherwise the maker's unmodified definitions.

Build target: `nice_nano_v2`, left and right shields. These UF2s are a software build check, not proof of electrical compatibility with an unidentified board revision. Verify exact PCB/controller/sensor with the maker before flashing, and keep a working recovery firmware. Do not flash `settings_reset` unless pairing recovery is actually needed; it wipes Bluetooth settings.
