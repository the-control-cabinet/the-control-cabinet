# The Control Cabinet

**Building automation and controls projects, built on real plant and documented to BMS standards: points lists, I/O schedules, commissioning and test records, fault diagnosis and decision logs.** I'm moving into **BMS / building automation engineering** after 25 years delivering business change programmes across financial services, insurance, telecoms and energy, with degrees in **Physics** and **Telecoms Engineering**.

📺 [The Control Cabinet on YouTube](https://www.youtube.com/channel/UC5Cupmz7vlfcodpCX7k8iuQ)

## In brief (one-minute read)

- **Real systems, not just labs.** A two-controller heating system (18 zones, radiators and underfloor, two unvented cylinders) integrated at radio-protocol level; mains water metered over Modbus RTU and field-calibrated; boiler-plant instrumentation on ESP32 controllers, with a designed OpenTherm control stage (weather compensation + PID, fail-safe changeover); fire/CO alarms interfaced through volt-free contacts; and a virtual pinball cabinet with real 24 V coils, layered protection and live current monitoring.
- **Protocols:** Modbus RTU and TCP, BACnet/IP, MQTT, Zigbee, Bluetooth LE, RAMSES-II (868 MHz), OpenTherm (design stage), plus SDR surveying of 433/868 MHz.
- **Engineering method:** every project has a points list or I/O schedule, a test record and an honest issues log. Faults are worked to root cause with evidence; for example, a permanent 5 °C override on both heating controllers was traced through eight tested hypotheses and packet-log analysis.
- **Head-end thinking:** a ~110-integration Home Assistant estate documented as a **BMS integration schedule** (protocol, local vs cloud, read vs write, resilience and command-authority tiers), plus a cyber-security and privacy baseline built on OT principles.

## Start here

| If you have five minutes | Why |
|---|---|
| [Evohome heating controls & RAMSES-II integration](https://github.com/the-control-cabinet/evohome-heating-controls-ramses-integration) | Real HVAC controls, protocol-level integration, a full fault case study |
| [Heating plant monitoring](https://github.com/the-control-cabinet/heating-plant-monitoring-esphome) | Plant-room points list, signal conditioning, boiler state detection; the measurement layer for the OpenTherm control design |
| [Mains water metering – Modbus RTU](https://github.com/the-control-cabinet/mains-water-metering-modbus-rtu) | Modbus RTU field device, calibration against measured volumes, metering dashboards |

## Skills matrix: BMS competencies mapped to evidence

| Competency | Where it's shown |
|---|---|
| **Points lists / I/O schedules** | [Plant monitoring](https://github.com/the-control-cabinet/heating-plant-monitoring-esphome) · [Water metering](https://github.com/the-control-cabinet/mains-water-metering-modbus-rtu) · [Aico interface](https://github.com/the-control-cabinet/aico-ei413-shelly-ha) · [VPin](https://github.com/the-control-cabinet/tukkari-vpin-real-mech-cabinet) · [Aircon DP map](https://github.com/the-control-cabinet/localtuya-portable-aircon-dp-map) |
| **Modbus (RTU / TCP)** | [Water metering](https://github.com/the-control-cabinet/mains-water-metering-modbus-rtu) · [Modbus TCP collector](https://github.com/the-control-cabinet/modbus-tcp-data-collector) |
| **BACnet/IP** | [BACnet/IP explorer](https://github.com/the-control-cabinet/bacnet-ip-network-explorer) |
| **HVAC controls** | [Evohome](https://github.com/the-control-cabinet/evohome-heating-controls-ramses-integration) · [Plant monitoring](https://github.com/the-control-cabinet/heating-plant-monitoring-esphome) · [OpenTherm control](https://github.com/the-control-cabinet/opentherm-boiler-control-esphome) · [Air quality / DCV](https://github.com/the-control-cabinet/indoor-air-quality-monitoring) |
| **Control strategy (PID, weather compensation, interlocks)** | [OpenTherm control](https://github.com/the-control-cabinet/opentherm-boiler-control-esphome) |
| **Commissioning and test records** | Every project: test tables, calibration runs, transmit audits · plans: [OpenTherm 12-test plan](https://github.com/the-control-cabinet/opentherm-boiler-control-esphome) · [BLE receiver calibration](https://github.com/the-control-cabinet/esp32-ble-presence-network) |
| **Fault diagnosis** | [5 °C override case study](https://github.com/the-control-cabinet/evohome-heating-controls-ramses-integration) · [Water meter calibration](https://github.com/the-control-cabinet/mains-water-metering-modbus-rtu) · [Zigbee availability noise](https://github.com/the-control-cabinet/zigbee-network-migration-z2m) · [ESPHome watchdog resets](https://github.com/the-control-cabinet/esp32-ble-presence-network) |
| **Life-safety interfaces** | [Fire/CO interface](https://github.com/the-control-cabinet/aico-ei413-shelly-ha) · [Layered leak detection](https://github.com/the-control-cabinet/layered-leak-detection) |
| **Metering and energy** | [Water metering](https://github.com/the-control-cabinet/mains-water-metering-modbus-rtu) · [Energy dashboard](https://github.com/the-control-cabinet/home-energy-dashboard) |
| **Signal conditioning and field wiring** | [Plant monitoring](https://github.com/the-control-cabinet/heating-plant-monitoring-esphome) · [VPin power and protection](https://github.com/the-control-cabinet/tukkari-vpin-real-mech-cabinet) |
| **Wireless field networks and RF** | [Zigbee](https://github.com/the-control-cabinet/zigbee-network-migration-z2m) · [BLE presence](https://github.com/the-control-cabinet/esp32-ble-presence-network) · [RTL-SDR survey](https://github.com/the-control-cabinet/rtl-sdr-rf-exploration) |
| **Head-end / integration management** | [HA integration schedule](https://github.com/the-control-cabinet/home-assistant-integration-schedule) |
| **OT cyber security** | [Security baseline](https://github.com/the-control-cabinet/smart-home-security-baseline) |

## Portfolio: top down

### Management level
| Project | Status |
|---|---|
| [Home Assistant integration schedule (~110 integrations, head-end documentation)](https://github.com/the-control-cabinet/home-assistant-integration-schedule) | ✅ Live |
| [Smart-home cyber-security & privacy baseline (OT principles)](https://github.com/the-control-cabinet/smart-home-security-baseline) | ✅ Live |
| [Whole-home energy & utility metering dashboard](https://github.com/the-control-cabinet/home-energy-dashboard) | 📐 Planned |
| HA + Node-RED supervisory controller | In progress |
| Alarm and trend strategy | Planned |
| Niagara / Tridium familiarisation | Planned |

### Automation level
| Project | Status |
|---|---|
| [Indoor air quality monitoring + demand-controlled ventilation](https://github.com/the-control-cabinet/indoor-air-quality-monitoring) | 🚧 In progress |
| [Layered leak detection](https://github.com/the-control-cabinet/layered-leak-detection) | 🚧 Partly live |
| [AI vision automations (vision as a sensor)](https://github.com/the-control-cabinet/ai-vision-automations) | ✅ Live (local detection planned) |
| [Fault diagnosis case study – Evohome permanent 5 °C override](https://github.com/the-control-cabinet/evohome-heating-controls-ramses-integration#4-part-c--fault-case-study-the-permanent-5-c-override) | ✅ Complete |
| [Tukkari VPin – real-mech cabinet (power, protection, I/O, instrumentation)](https://github.com/the-control-cabinet/tukkari-vpin-real-mech-cabinet) | ✅ Running |
| Multi-zone optimum start/stop | Planned |
| Duty/standby pump rotation | In progress |
| [OpenTherm boiler control – weather comp + PID with anti-hunt, alongside two Evohome controllers](https://github.com/the-control-cabinet/opentherm-boiler-control-esphome) | 📐 Design stage |
| Plant state machine and interlocks | Planned |
| Trend IQ411 commissioning | Planned |
| PLC re-implementation (TIA Portal / CODESYS) | Planned |

### Field level
| Project | Status |
|---|---|
| [Evohome heating controls & HA integration (cloud → RAMSES-II, incl. fault case study)](https://github.com/the-control-cabinet/evohome-heating-controls-ramses-integration) | ✅ Complete |
| [Heating plant monitoring – boiler, cylinders, safety devices (ESPHome)](https://github.com/the-control-cabinet/heating-plant-monitoring-esphome) | 🚧 In progress |
| [Mains water metering – Modbus RTU](https://github.com/the-control-cabinet/mains-water-metering-modbus-rtu) | ✅ Complete |
| [Modbus TCP data collector](https://github.com/the-control-cabinet/modbus-tcp-data-collector) | ✅ Complete |
| [BACnet/IP network explorer](https://github.com/the-control-cabinet/bacnet-ip-network-explorer) | ✅ Complete |
| [Fire & CO alarm interface – Aico Ei413 → Shelly → HA](https://github.com/the-control-cabinet/aico-ei413-shelly-ha) | ✅ Complete |
| [Portable aircon – Tuya data-point map, local control](https://github.com/the-control-cabinet/localtuya-portable-aircon-dp-map) | ✅ Complete |
| [Zigbee network migration – ZHA → Zigbee2MQTT (93 devices)](https://github.com/the-control-cabinet/zigbee-network-migration-z2m) | ✅ Complete |
| [ESP32 BLE presence network](https://github.com/the-control-cabinet/esp32-ble-presence-network) | ✅ Live |
| [RTL-SDR RF survey – 433/868 MHz](https://github.com/the-control-cabinet/rtl-sdr-rf-exploration) | ✅ Exploratory |
| Water sub-metering by event detection (shower, washing machine) | Next |
