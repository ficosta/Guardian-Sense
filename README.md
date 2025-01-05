# GuardianSense

**GuardianSense** is a versatile hardware project based on the ESP32-S3, designed to monitor environmental conditions and provide real-time data to **Zabbix**. This board is compact yet powerful, integrating multiple sensors for a wide range of applications, including data centers, smart homes, and industrial environments.

## Features

- **Core Module**: ESP32-S3-WROOM-1 for Wi-Fi and BLE connectivity.
- **Environmental Sensors**:
  - Temperature and Humidity (BME280)
  - Smoke Detection (MQ-2)
  - Light Intensity (BH1750)
  - Presence Detection (AM312 PIR Sensor)
  - Vibration Monitoring (LDT0-028K)
  - Noise Level Monitoring (MAX9814)
- **Indicators**:
  - Status LED (Single color)
  - RGB LED (SK6812-MINI-E)
- **Connectivity**:
  - USB-C for power and data
  - Multiple GPIOs for additional customizations
- **Power Management**:
  - Integrated voltage regulator for 3.3V operation.

## Firmware

The firmware for GuardianSense is tailored to interact with **Zabbix**, providing seamless integration with this monitoring platform. It supports real-time data transmission for:

- Temperature and humidity
- Smoke and gas levels
- Light intensity
- Vibration and noise detection

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/ficosta/Guardian-Sense.git
   ```

2. Install KiCad for hardware design modifications (optional).

3. Flash the firmware to the ESP32-S3 module.

4. Configure Zabbix to accept incoming data from the board.

## KiCad Design Files

All hardware design files for GuardianSense are included in the `/hardware` directory. Make sure to follow the project's **.gitignore** for KiCad files when contributing.

## Contributing

Contributions are welcome! Please ensure that any hardware or firmware changes align with the project's goals.

## License

See the `LICENSE` file for more details.
