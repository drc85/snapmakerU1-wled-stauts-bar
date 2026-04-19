# snapmakerU1-wled-stauts-bar
wled stauts bar for the snapmakerU1

Based on WLED (https://github.com/Aircoookie/WLED)
and Klipper API integration.

Modified and extended by [drc85]

download firmware.bin and flash it to your esp32 and setup up the network connection

inside wled usermod there is a new window

<img width="529" height="261" alt="image" src="https://github.com/user-attachments/assets/6a229949-6cae-4b88-bab5-454d0fce1067" />

enter your printer ip here, if necceary ur auth api, if u dont have auth - leave empty


after reboting it wil show the status like this...


## LED Status Overview

- 🔵 **Idle / Standby**  
  Solid cyan-blue (soft light)

- 🟡 **Preparing / Preheat / Calibration**  
  Smooth pulsing orange (remains active until printing actually starts, including bed leveling and filament loading)

- 🟢 **Printing**  
  Apple-style green progress bar (16 LEDs)  
  - Smooth gradient with a bright moving head  
  - Always shows at least 1 LED, even at very low progress

- 🔵 **Paused**  
  Soft pulsing blue (distinct from idle and heating)

- 🔴 **Error**  
  Flashing red (dim ↔ bright, never fully off)

- 🟢 **Complete (Finished)**  
  Flashing green for ~10 seconds, then returns to idle


