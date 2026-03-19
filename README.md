# wndr4300sw

Patch tool that converts Netgear WNDR4300 firmware images to run on the WNDR4300SW hardware variant.

## What It Does

Replaces the 128-byte device header in a WNDR4300 firmware binary (`V1.0.0.6`) with the WNDR4300SW header, allowing the image to be flashed on the SW model.

## Usage

```c
gcc -o patch4300SW patch4300V1.0.0.6SW.c
./patch4300SW file.img
```

**Warning:** The file is converted in place.