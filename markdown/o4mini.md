# IoT Exam Preparation Guide

This README synthesizes all core concepts, architectures, protocols, security practices, and industry use cases from your provided IoT materials. Use it as a roadmap—dive deeper into any section by reviewing your PDFs, lecture notes, and slides.

---

## Table of Contents

1. Overview & Exam Strategy
2. Core IoT Concepts
3. IoT Reference Architectures
4. Smart Objects (Things)
5. Connectivity & Networking
6. IP in Constrained Networks
7. Application Protocols
8. Data Management & Analytics
9. Security in IoT
10. Industry-Specific Use Cases
11. Industrial Automation Fundamentals
12. Study Tips & Glossary

---

## 1. Overview & Exam Strategy

- **Goal:** Understand _why_ each technology/architecture is used, not just _what_ it is.
- **Approach:**
  1. Build from bottom-up: Things → Network → Protocols → Analytics → Applications → Security → Use Cases.
  2. Redraw key diagrams (IoT stacks, Purdue model, protocol flows).
  3. Compare & contrast alternatives (e.g., CoAP vs. MQTT, LoRaWAN vs. NB-IoT).
  4. Relate theory to real-world examples in each industry domain.
  5. Use flashcards for acronyms and protocol parameters.

---

## 2. Core IoT Concepts

- **Definition & Scope:**

  - Connecting “things” (sensors, actuators, smart objects) to collect data and/or effect physical changes.
  - Enables digitization and automation across domains.

- **Key Drivers:**

  - Scale (billions of devices → IPv6)
  - Constrained resources (CPU, memory, power, bandwidth)
  - Legacy integration
  - Real-time/low-latency requirements
  - Security & privacy challenges
  - Big data volumes and analytics needs

- **IT vs. OT Convergence:**
  - IT focuses on confidentiality, integrity, availability (CIA).
  - OT prioritizes availability, integrity, safety (A-I-C).
  - Legacy OT systems often “air-gapped” but now increasingly networked.

---

## 3. IoT Reference Architectures

1. **oneM2M** – Standard service layer for M2M interoperability.
2. **IoTWF 7-Layer Model:**
   1. Physical/Controllers
   2. Connectivity
   3. Edge/Fog Computing
   4. Data Accumulation
   5. Data Abstraction
   6. Application
   7. Collaboration/Processes
3. **Simplified 3-Layer Stack:**
   - Layer 1: Things (Sensors/Actuators)
   - Layer 2: Communications (Access, Gateways, Transport, Management)
   - Layer 3: Applications & Analytics
4. **Purdue Enterprise Reference Architecture (PERA):**

   - Levels 0–5: Field devices → Control → Supervisory → DMZ → Enterprise.
   - Enforces separation of IT/OT zones via DMZ.

5. **Compute Hierarchy:**
   - Edge (device-level) → Fog (local aggregation/processing) → Cloud (global services).

---

## 4. Smart Objects (Things)

- **Sensors:**

  - Classify by active/passive, invasive/non-invasive, absolute/relative, physical variable (temperature, pressure, etc.).
  - Constraints: low power, limited compute, intermittent connectivity.

- **Actuators:**

  - Convert digital commands to physical actions (motors, valves, relays).

- **MEMS:**

  - Micro-Electro-Mechanical Systems integrating sensors + actuators on a chip.

- **Wireless Sensor Networks (WSNs):**
  - Self-organizing meshes, often built on IEEE 802.15.4.

---

## 5. Connectivity & Networking

### 5.1 Criteria & Topologies

- **Range Categories:** Short (<100 m), Medium (1 km), Long (>10 km)
- **Frequency Bands:**

  - Unlicensed ISM: 2.4 GHz, sub-GHz (868 MHz EU, 915 MHz US)
  - Licensed: cellular LPWA

- **Topologies:** Star, Mesh, Peer-to-Peer
- **Power Modes:** Always-on vs. power-cycled (battery-powered)
- **Constrained Node Classes (RFC 7228):**
  - Class 0: <10 KB RAM
  - Class 1: ~50 KB RAM
  - Class 2: ~250 KB RAM

### 5.2 Key Wireless Standards

- **IEEE 802.15.4:** PHY/MAC for low-rate WPAN. Basis for ZigBee, 6LoWPAN, Thread, WirelessHART.
- **IEEE 802.15.4g/e:** Enhancements for Smart Utility Networks (SUN) and TSCH (time-slotted MAC).
- **IEEE 802.11ah (HaLow):** Sub-1 GHz Wi-Fi for IoT (longer range, lower data rate).
- **Power-Line Communication (PLC):** IEEE 1901.2a, G3-PLC, PRIME for smart metering.
- **LPWA Technologies:**
  - **LoRaWAN:** Chirp Spread Spectrum, star-of-stars, OTAA/ABP, Class A/B/C devices.
  - **Sigfox, Ingenu, NB-IoT, LTE-M:** Trade-offs in bandwidth, battery life, cost, QoS.

---

## 6. IP in Constrained Networks

- **Why IP?** Interoperability, end-to-end addressing, leverage existing infrastructure.

- **6LoWPAN:**

  - Header compression (stateless, stateless + context), fragmentation, mesh-under vs. mesh-over.

- **6TiSCH:**

  - IPv6 on TSCH (802.15.4e), 6top scheduling, track-based vs. distributed scheduling.

- **RPL (Routing Protocol for LLNs):**
  - Constructs Destination-Oriented DAGs (DODAGs), uses DIO/DAO messages, supports storing/non-storing modes, objective functions (ETX, latency).

---

## 7. Application Protocols

### 7.1 Legacy & Web Protocols

- **SCADA Protocols over IP:** Modbus/TCP, DNP3/IP, IEC 60870-5-104 via tunneling or protocol translation.
- **HTTP/HTTPS, REST vs. SOAP:** Heavyweight for constrained nodes.

### 7.2 IoT-Optimized Protocols

- **CoAP (Constrained Application Protocol):**

  - UDP-based, RESTful (GET/POST/PUT/DELETE), message types: CON, NON, ACK, RST; block-wise transfer; resource discovery (`/.well-known/core`); Observe pattern.

- **MQTT:**

  - TCP-based publish/subscribe; broker mediates topics; QoS 0/1/2; lightweight CONNECT/PUBLISH/SUBSCRIBE/PING.

- **Comparisons:**
  - CoAP: request/response, UDP, lower header overhead.
  - MQTT: pub/sub, TCP, persistent sessions, higher overhead but reliable streams.

---

## 8. Data Management & Analytics

- **IoT Big Data Characteristics:** Volume, Velocity, Variety (3 Vs).
- **Analytics Types:** Descriptive, Diagnostic, Predictive, Prescriptive.
- **Machine Learning:**

  - Supervised (classification, regression), unsupervised (clustering), neural networks, deep learning.
  - Edge vs. cloud training/inference trade-offs.

- **Big Data Ecosystem:**

  - **HDFS & MapReduce**, **YARN**, **Kafka**, **Spark (Streaming, MLlib)**, **Storm**, **Flink**.
  - **Lambda Architecture:** Batch + speed + serving layers.

- **Edge/Fog Analytics:** Real-time stream processing at network edge—reduces latency and bandwidth use.
- **Network Analytics:** IPFIX/Flexible NetFlow for traffic profiling, anomaly detection, capacity planning.

---

## 9. Security in IoT

- **OT vs. IT Security Posture:**

  - OT values continuous operations and safety; IT values data confidentiality and integrity.

- **Purdue Model Zones:**

  - Level 0–1 (field devices), Level 2–3 (control & supervisory), Level 4–5 (enterprise).
  - Enforce DMZ between IT/OT, strict ACLs and segmentation.

- **Risk Management Frameworks:**

  - **OCTAVE Allegro:** Asset-centric threat identification.
  - **FAIR:** Quantitative risk modeling (frequency, magnitude).

- **Security Controls:**

  - Inventory & asset discovery; network segmentation; secure protocols (TLS, DTLS, MACsec); VPNs; device certificate management; IDS/IPS; anomaly detection.

- **Constrained Device Security:**
  - IETF ACE (Authentication and Authorization for Constrained Environments), DICE (Device Identity Composition Engine).

---

## 10. Industry-Specific Use Cases

### 10.1 Manufacturing (Industry 4.0)

- **CPwE (Converged Plantwide Ethernet)** architecture
- **IACS:** PLCs, DCS, SCADA integration
- **Protocols:** EtherNet/IP, PROFINET, Modbus/TCP, OPC UA
- **Resiliency:** REP, HSR, PRP
- **Security:** IDMZ, network segmentation, NAC

### 10.2 Oil & Gas

- **Life-Cycle:** Upstream (exploration), Midstream (transport), Downstream (refining)
- **Wireless Field Area Networks**, satellite backhaul, ruggedized devices
- **Security:** Remote access control, anomaly detection, patch management

### 10.3 Utilities (Smart Grid)

- **GridBlocks Model**, Smart Substation Automation (IEC 61850, GOOSE, SV, MMS)
- **Teleprotection:** Distance and current differential relays, MPLS-TP
- **Field Area Networks:** AMI, DA, DR
- **Compliance:** NERC CIP standards

### 10.4 Smart Cities

- **Architecture Layers:** Street (sensors/actuators), network, data center, service bus, applications
- **Use Cases:** Intelligent lighting, parking, traffic management, environmental monitoring
- **Security & Privacy:** Data anonymization, secure API gateways

### 10.5 Transportation

- **Roadways (V2X):** DSRC/WAVE, C-V2X, cellular fallback
- **Fleet Management:** Telematics, GPS, fuel and maintenance monitoring
- **Mass Transit & Rail:** CBTC, PTC, wireless mesh for onboard and wayside systems

### 10.6 Public Safety

- **Mission Continuum:** Emergency dispatch, mobile command units, on-scene networks
- **Collaboration:** Interagency data sharing, robust mesh networking, priority QoS
- **Edge Analytics:** Real-time video, health monitoring, situational awareness

---

## 11. Industrial Automation Fundamentals

- **PLCs:** Real-time control loop, scan cycle (Input → Logic → Output → Housekeeping), modular I/O.
- **SCADA:** Supervisory computers, RTUs/PLCs, HMI, long-haul communications.
- **LabVIEW:** Graphical dataflow programming, integration with OPC UA for device interoperability.

---

## 12. Study Tips & Glossary

- **Active Recall:** Teach concepts aloud or write them from memory.
- **Flashcards:** Acronyms & definitions (e.g., LPWA, LLN, FOG, DODAG, OPC UA, QOS).
- **Diagram Practice:** Sketch stacks, message flows (CoAP, MQTT), network zones.
- **Time Allocation:** Prioritize areas emphasized by your instructor.

Glossary of Key Acronyms:  
LPWA, ISM, WSN, 6LoWPAN, RPL, TSCH, CoAP, MQTT, DNP3, OPC UA, HMI, PLC, SCADA, DMZ, CPwE, IACS, GOOSE, SV, AMI, NERC, V2X.
