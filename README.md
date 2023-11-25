# powerreporter

My first projet with ESPHOME:
* Connects SofarSolar ME3000 inverter to Home Assistant
* Connects also linky power meter to Home Assistant
* Displays ME3000 info: solar, import, export, totals, T°, battery % ...

# How to compile
* Install esphome environnement
* Clone repository
* Copy secrets-templates.yaml to secrets.yaml edit the file to mathc your SSID and password
* Connect ESP32 board
* Type "esphome run powerreporter-s2.yaml"
