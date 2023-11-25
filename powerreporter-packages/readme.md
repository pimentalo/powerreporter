# Fichiers pour le ME3000 sous esphome

Les fichiers sont basés sur ce genre de configuration:

uart:
  id: mod_bus
  tx_pin: 17
  rx_pin: 16
  baud_rate: 115200
  stop_bits: 1

modbus:
  flow_control_pin: 5
  id: modbus1

modbus_controller:
  - id: sofarME3000
    ## the Modbus device addr
    address: 0x1
    modbus_id: modbus1
    setup_priority: -10

text_sensor: !include me3000/me3000-text_sensor.yaml
sensor: !include me3000/me3000-sensor.yaml
binary_sensor: !include me3000/me3000-binary_sensor.yaml
