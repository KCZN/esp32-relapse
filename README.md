# esp32-webkit
__only tested with ESP32-arduino.pico.merged.bin__ as of 14/10/2026

projects used/referenced:
<br>
https://github.com/ntfargo/Relapse-Exploit
<br>
^^ Relapse (I used the original release)
<br>
<br>
https://github.com/owendswang/ps5-webkit-autoloader-esp32/tree/main
<br>^^ the entire foundation. read this if you are unsure if you need a standard or debug image to flash!

# How to use
- flash the appropriate .bin to your esp device
- connect esp to ps5 and connect to its WiFi (ESP32_PORTAL)
<br>PASSWORD: 12345678 (should be)
- open settings, first tab and click on user guide
- press OK when prompted
- profit.

one minor issue is you will need to close settings and open it again for debug settings to actually appear.

# sending payloads
connect to the esp32's wifi on your pc, phone or whatever and then send payloads to esp_ip:9021 using your preferred method.

# How to build/edit src
You must use make, install arduino cli and core 2.0.1.1 for it as these are dependencies. Go into project root, open terminal and type 'make', it'll produce several folders inside /build/, out of all the produced files inside each board types folder, you only care to flash the ESP32-arduino.x.merged.bin file to your respective board matching it. 

# DISCLAIMER
I did not code anything here, I threw together two different things and made it work. All rights/thanks go to the original developers!
