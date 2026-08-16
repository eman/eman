Python developer working on home energy monitoring and IoT. Most of my open-source work is device libraries, Home Assistant integrations, and ESPHome components for HVAC and plumbing hardware that I have in my home.

---

## Projects

[<img src="https://raw.githubusercontent.com/eman/tariffkit/main/images/banner.svg" alt="TariffKit" width="420">](https://github.com/eman/tariffkit)
#### [TariffKit](https://github.com/eman/tariffkit)

Offline electricity tariff engine for pricing imports and exports, forecasting rates, and calculating bills from interval meter data. TariffKit ships as a Python library and CLI, with REST, MQTT, and Home Assistant integrations built on the same table-driven engine; its first data provider covers PG&E residential tariffs, NBT export compensation, and California Community Choice Aggregators.

[![Navien NWP500 Banner](images/banner_small.svg)](https://github.com/eman/ha_nwp500)
#### [Python library](https://github.com/eman/nwp500-python) / [Home Assistant integration](https://github.com/eman/ha_nwp500)

Python library and Home Assistant integration for the Navien NWP500 heat pump water heater. The library communicates over the Navien cloud API and a local MQTT connection for real-time state. The HA integration exposes full control (temperature setpoint, operation modes, power), energy tracking, safety sensors (leak detection, freeze protection, scald warnings), and a reservation scheduling service for time-based mode changes.

### Grundfos ALPHA HWR — [Python library](https://github.com/eman/alpha-hwr)

Python library and CLI for the Grundfos ALPHA HWR domestic hot water recirculation pump via Bluetooth Low Energy. Supports automatic pump discovery and pairing, real-time telemetry streaming (flow, pressure, power, temperature), all five primary control modes (temperature control with AUTOADAPT, cycle time, constant curve/pressure/flow), schedule management, and full configuration backup and restore. Published to PyPI; async-first and built on Pydantic.

### Grundfos ALPHA HWR — [ESPHome component](https://github.com/eman/esphome-alpha-hwr)

ESPHome C++ components and YAML packages for the same hardware. Two components: `alpha_hwr` for BLE telemetry and control of the Grundfos ALPHA HWR, and `dhw_demand` for on-device domestic hot water demand detection using pump telemetry and/or Home Assistant sensors. Ships reusable package YAML so external ESPHome configs can pull the component stack directly from GitHub. Also includes an optional Lovelace schedule card for managing weekly pump schedules from Home Assistant.

[<img src="https://raw.githubusercontent.com/eman/homeassistant-quilt-hp/main/images/banner.svg" alt="Quilt Home Assistant Integration" width="420">](https://github.com/eman/homeassistant-quilt-hp)
#### [Python library](https://github.com/eman/quilt-hp-python) / [Home Assistant integration](https://github.com/eman/homeassistant-quilt-hp)

Python client library and Home Assistant integration for Quilt mini-split HVAC systems. The library communicates with the Quilt cloud API via gRPC and supports controlling spaces and indoor units, comfort presets, schedules, energy usage queries, and real-time state streaming. The HA integration builds on that client to expose climate/fan/light/select/sensor entities in Home Assistant with OTP auth, multi-home support, and real-time updates with polling fallback.

### Eagle Home Energy Gateway — [Python library](https://github.com/eman/meter_reader)

Python library and CLI for retrieving near-realtime energy usage from a smart meter via the Eagle Home Energy Gateway. Supports instantaneous demand, demand history, and summation values over configurable time intervals. No external dependencies; outputs as table, JSON, or CSV.

---

**Languages:** Python, Go, C++  
**Platforms:** Home Assistant, ESPHome, InfluxDB
