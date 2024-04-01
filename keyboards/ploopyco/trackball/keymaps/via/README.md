# Ploopy Trackball Classic
https://ploopy.co/classic-trackball/

## Instructions
Follow these instructions to flash updated firmware, keymaps, etc. using QMK.

1. Make any changes to firmware files first.
2. Open Windows terminal and open the QMK MSYS profile.
3. Build the firmware with:
    ```
    qmk compile -kb ploopyco/trackball/rev1_005 -km via
    ```

    This sets the Ploopy up for Via, so use that for keymaps:
    https://usevia.app

4. Put the Ploopy into bootloader mode (see below).
5. Flash using the QMK Toolbox: https://github.com/qmk/qmk_toolbox

All done!

## Putting the Ploopy Trackball into bootloader mode
Instructions from: https://github.com/ploopyco/classic-trackball/wiki/Appendix-C:-QMK-Firmware-Programming#putting-the-ploopy-trackball-into-bootloader-mode

1. Unplug it from your computer.
2. If you're using a right-handed Ploopy Classic, hold the "back" button. This is the button just to the right of the ball; it normally sits under your ring (fourth) finger. If you're using a left-handed Ploopy Classic, hold the "forward" button.
3. While holding the button, plug the Ploopy Trackball into your computer. If you're using QMK Toolbox, it should show up in the console. If using dmesg, it'll show up as an Atmel DFU device.

And that's it. While plugged in this way, the Ploopy Trackball will accept new firmware.

## Links
- https://github.com/ploopyco/classic-trackball/wiki/Appendix-C:-QMK-Firmware-Programming
- https://docs.qmk.fm/#/newbs_building_firmware
- https://docs.qmk.fm/#/newbs_flashing
