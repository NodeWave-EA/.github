<a href="https://www.nodewave.net">
  <img src="./logo.svg" alt="NodeWave — Smart IoT Solutions" width="336" height="96"></img>
</a>

End-to-end IoT engineering, industrial hardware, and connected infrastructure based in Nairobi, Kenya.

NodeWave EA focuses on practical Internet of Things (IoT) deployments across East Africa spanning custom PCB design, embedded firmware, industrial sensors and cellular gateways, edge computing, [signed Firmware-Over-The-Air (FOTA) management](https://fota.nodewave.net), and real-time cloud telemetry platforms.

---

## Core IoT Focus & Engineering Scope

- **Custom Hardware & Embedded Firmware:** Schematic capture, PCB layout, Design for Manufacture (DFM) review, weatherproof enclosure engineering, sensor calibration, and MCU firmware for ESP32, STM32, and cellular modems (C++, MicroPython, FreeRTOS).
- **Industrial IoT Hardware & Field Instrumentation:** Locally engineered backup power units (NodeWave B254KE series) alongside industrial 4G/LTE gateways, smart RTUs, radar level transmitters, flowmeters, and vibration/condition-monitoring systems via [nodewave.net/store](https://www.nodewave.net/store).
- **Connectivity & Edge Computing:** Multi-protocol field deployments over MQTT, CoAP, LoRaWAN, Modbus, BACnet, Zigbee, and cellular (4G LTE, LTE-M, NB-IoT) with local gateway rule execution, edge analytics, and offline store-and-forward buffering.
- **Cloud Ingestion, Security & Fleet Lifecycle:** Zero-trust device provisioning (mTLS/X.509 certificates and per-device JWT), time-series data pipelines, cryptographically verified FOTA rollouts, anomaly detection, and live operational dashboards.

---

## Open-Source & Public Repositories

| Repository | Description | Stack |
| :--- | :--- | :--- |
| [FOTA-Client-ESP32](https://github.com/Nodewave-EA/FOTA-Client-ESP32) | Secure ESP32 FOTA client with retry handling, post-boot health watchdog, lifecycle callbacks, and SHA-256 + ECDSA/ED25519/RSA signature verification. Published in the Arduino Library Registry. | C++ |
| [secure-iot-fota-platform-beta](https://fota.nodewave.net) | Staged firmware rollout and device fleet update management platform. | Nuxt 4, NestJS |
| [Dashboard-Demo](https://github.com/Nodewave-EA/Dashboard-Demo) | Reference implementation for live sensor telemetry, uptime tracking, and threshold alerts. | Nuxt 4 |
| [sensors.AFRICA.Mapv2](https://github.com/Nodewave-EA/sensors.AFRICA.Mapv2) | Continental air-quality sensor visualization map. | Vue 3 / Nuxt |
| [Nodewave Blogs](https://github.com/Nodewave-EA/Nodewave-Blogging-Website) | Technical documentation, engineering articles, and deployment case studies. | Nuxt 4 |

---

## Technical Stack

- **Microcontrollers & Edge:** ESP32, STM32, Raspberry Pi, C++, MicroPython, FreeRTOS, Node-RED, Docker
- **Protocols & Fieldbus:** MQTT, CoAP, LoRaWAN, Modbus, BACnet, Zigbee, 4G LTE, LTE-M, NB-IoT
- **Cloud, Web & Data:** AWS IoT, Nuxt 4, NestJS, InfluxDB, TimescaleDB, PostgreSQL, Grafana

---

## Sectors

- **Industrial Automation:** Machine condition monitoring, predictive maintenance, and factory floor telemetry.
- **Agriculture & Cold Chain:** Soil and microclimate sensing, automated irrigation control, and storage compliance logging.
- **Utilities & Environmental Monitoring:** Water distribution telemetry, air-quality sensor networks, and smart energy/backup power systems.
- **Supply Chain & Asset Tracking:** Geolocation telemetry, fleet diagnostics, and distributed facility monitoring.

---

## Contact & Operations

- **Website:** [nodewave.net](https://www.nodewave.net)
- **IoT Hardware Store:** [nodewave.net/store](https://www.nodewave.net/store)
- **FOTA Platform:** [fota.nodewave.net](https://fota.nodewave.net)
- **Engineering Blog:** [nodewave-blogs.vercel.app](https://nodewaveblog.vercel.app)
- **Technical Support:** [nodewave.net/contact](https://www.nodewave.net/contact)
- **General Inquiries:** info@nodewave.net
- **Security Disclosures:** security@nodewave.net
- **Location:** Falcon Road, off Enterprise Road, Industrial Area, Nairobi, Kenya

---

## Contributing & Licensing

Contributions to our open-source libraries and tools are welcome. Review our [Contributing Guidelines](.github/CONTRIBUTING.md) and [Code of Conduct](.github/CODE_OF_CONDUCT.md) before opening a pull request.

Licensing varies by project; refer to the `LICENSE` file in each individual repository.
