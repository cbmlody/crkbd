# Crkbd custom firmware repository

## To be used with QMK cli

### Install
1. install QMK MSYS
2. Open QMK MSYS and run 
```bash
qmk setup
```
3. copy files from QMK folder to
```bash
%userprofile%/qmk_firmware/keyboards/crkbd/<folder>
```
4. Run build command in QMK MSYS
```bash
qmk compile -c -kb crkbd/<folder> -km default -e CONVERT_TO=promicro_rp2040
```
5. This will produce files in `%userprofile%/qmk_firmware/.build`. This is compiled for RP2040 MCU so you have to copy `*.uf2` file to your MCU in boot mode.
