# Free Fire Sensitivity Generator

## Current State
App generates Free Fire sensitivity settings based on device name. Has DPI selector (120-600) and fixed fire button size of 200.

## Requested Changes (Diff)

### Add
- DPI recommendation (1–1000) derived from device tier when user enters device name
- Fire button size recommendation (1–100) derived from device tier when user enters device name

### Modify
- Remove manual DPI selector; instead show recommended DPI value (1–1000) based on device name
- Fire button size now shown as recommended value (1–100) instead of fixed 200
- All sensitivity values still 0–200 range, auto-scaled based on recommended DPI

### Remove
- Manual DPI range slider (120–600)
- Fixed fire button size of 200

## Implementation Plan
1. Update device tier mapping to include DPI (1–1000) and fire size (1–100) recommendations
2. Display recommended DPI and fire size as output cards after device name entry
3. Scale sensitivity values based on recommended DPI
4. Update UI to show all recommendations clearly
