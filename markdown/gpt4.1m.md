# IoT Exam Study Guide

This is a very highly detailed README/Study Guide for your IoT exam, based on the content and structure of the "IoT Fundamentals" textbook and the slide decks you referenced. This guide is organized for deep understanding, quick review, and practical exam preparation.

---

## Table of Contents

- [IoT Exam Study Guide](#iot-exam-study-guide)
  - [Table of Contents](#table-of-contents)
  - [Introduction \& Exam Strategy](#introduction--exam-strategy)
  - [Core IoT Concepts](#core-iot-concepts)
  - [IoT Reference Architectures](#iot-reference-architectures)
    - [IoTWF 7-Layer Model](#iotwf-7-layer-model)
    - [Purdue Model](#purdue-model)
    - [Simplified 3-Layer Stack](#simplified-3-layer-stack)
  - [Smart Objects: Sensors \& Actuators](#smart-objects-sensors--actuators)
  - [IoT Connectivity \& Networking](#iot-connectivity--networking)
    - [Criteria](#criteria)
    - [Key Technologies](#key-technologies)
  - [IP Networking in IoT](#ip-networking-in-iot)
  - [IoT Application Protocols](#iot-application-protocols)
  - [Data Management \& Analytics](#data-management--analytics)
  - [IoT Security](#iot-security)
  - [Industry Use Cases](#industry-use-cases)
    - [Manufacturing](#manufacturing)
    - [Oil \& Gas](#oil--gas)
    - [Utilities (Smart Grid)](#utilities-smart-grid)
    - [Smart Cities](#smart-cities)
    - [Transportation](#transportation)
    - [Public Safety](#public-safety)
  - [Industrial Automation Fundamentals](#industrial-automation-fundamentals)
  - [Exam Preparation Tips](#exam-preparation-tips)

---

## Introduction & Exam Strategy

- **Purpose:** This guide synthesizes your course’s key IoT concepts, protocols, architectures, and real-world applications.
- **How to Use:**
  - Read actively, not passively.
  - Draw diagrams from memory.
  - Make comparison tables.
  - Practice scenario-based questions.
  - Use flashcards for acronyms and protocol features.

---

## Core IoT Concepts

- **Definition:** IoT is the networked interconnection of physical objects (“things”) embedded with sensors, software, and connectivity to collect and exchange data.
- **Key Drivers:**
  - Scale (billions of devices)
  - Constrained resources (power, memory, bandwidth)
  - Real-time data and analytics
  - Security and privacy
  - Integration of legacy systems
- **IT vs. OT:**
  - IT: Focus on Confidentiality, Integrity, Availability (CIA)
  - OT: Focus on Availability, Integrity, Safety (AIC)
  - Convergence challenges: update cycles, security priorities, data types

---

## IoT Reference Architectures

### IoTWF 7-Layer Model

1. **Physical Devices & Controllers:** Sensors, actuators, edge devices
2. **Connectivity:** Wired/wireless protocols (e.g., ZigBee, LoRaWAN)
3. **Edge Computing:** Local data processing, latency reduction
4. **Data Accumulation:** Storage, aggregation
5. **Data Abstraction:** Normalization, APIs
6. **Applications:** Business logic, analytics
7. **Collaboration & Processes:** Integration with enterprise systems

### Purdue Model

- **Levels 0–5:** Field devices (0) to enterprise IT (5)
- **DMZ:** Demilitarized zone between IT and OT

### Simplified 3-Layer Stack

- **Things → Network → Applications/Analytics**

---

## Smart Objects: Sensors & Actuators

- **Sensors:**
  - Types: Active/passive, invasive/non-invasive, contact/no-contact, absolute/relative
  - Examples: Temperature, pressure, motion, humidity
- **Actuators:**
  - Types: Motors, relays, valves
- **MEMS:** Micro-Electro-Mechanical Systems (miniaturized sensors/actuators)
- **Smart Objects:** Devices with processing, sensing/actuation, communication, and power
- **Trends:** Smaller, lower power, more processing, better comms, more standardization

---

## IoT Connectivity & Networking

### Criteria

- **Range:** Short (ZigBee), Medium (Wi-Fi), Long (LoRaWAN, NB-IoT)
- **Frequency Bands:** ISM (2.4 GHz, sub-GHz), licensed/unlicensed
- **Power:** Always-on vs. battery-powered (LPWA)
- **Topology:** Star, mesh, peer-to-peer
- **Constrained Devices:** RFC 7228 Classes 0, 1, 2

### Key Technologies

- **IEEE 802.15.4:** Foundation for ZigBee, 6LoWPAN, Thread, WirelessHART
- **IEEE 802.15.4g/e:** Smart Utility Networks, TSCH MAC
- **IEEE 1901.2a:** Power Line Communication (NB-PLC)
- **IEEE 802.11ah (HaLow):** Sub-GHz Wi-Fi for IoT
- **LoRaWAN:** Long-range, low-power, star-of-stars topology, classes A/B/C
- **NB-IoT/LTE-M:** Cellular LPWA, licensed spectrum

---

## IP Networking in IoT

- **Why IP?** Open, scalable, interoperable, manageable, secure
- **6LoWPAN:** IPv6 over low-power wireless (header compression, fragmentation, mesh-under/mesh-over)
- **6TiSCH:** IPv6 over TSCH (time-slotted channel hopping)
- **RPL:** Routing Protocol for LLNs (DODAGs, DIO/DAO, storing/non-storing, ETX metric)
- **Adoption vs. Adaptation:** Direct IP vs. protocol translation/gateways

---

## IoT Application Protocols

- **Transport Layer:**
  - TCP: Reliable, higher overhead
  - UDP: Lightweight, less reliable, used in constrained networks
- **CoAP:**
  - UDP-based, RESTful, low overhead, resource discovery, block-wise transfer, DTLS security
- **MQTT:**
  - TCP-based, publish/subscribe, brokered, QoS 0/1/2, TLS security
- **SCADA Protocols:** Modbus/TCP, DNP3/IP, IEC 60870-5-104 (legacy adaptation)
- **HTTP/HTTPS, XMPP:** For less-constrained devices

---

## Data Management & Analytics

- **Big Data Challenges:** Volume, velocity, variety
- **Data Types:** Structured (relational), unstructured (NoSQL)
- **Analytics Types:**
  - Descriptive (what happened)
  - Diagnostic (why)
  - Predictive (what will happen)
  - Prescriptive (what should be done)
- **Machine Learning:**
  - Supervised (classification, regression)
  - Unsupervised (clustering, anomaly detection)
  - Edge vs. cloud ML
- **Tools:** Hadoop (HDFS, MapReduce), Spark, Kafka, Storm, Flink, Lambda architecture
- **Edge/Fog Analytics:** Real-time, local processing, bandwidth reduction

---

## IoT Security

- **OT Security History:** Stuxnet, Maroochy Shire, Ukraine grid attack
- **Challenges:** Legacy systems, insecure protocols, device vulnerabilities, vendor lock-in
- **IT vs. OT Security:** CIA vs. AIC/Safety, different priorities and approaches
- **Risk Analysis:**
  - OCTAVE Allegro (asset-centric)
  - FAIR (quantitative, frequency × magnitude)
- **Best Practices:**
  - Segmentation (zones/conduits, DMZ)
  - Secure comms (VPN, MACsec, TLS/DTLS)
  - IDS/IPS, anomaly detection
  - Patch management, asset inventory

---

## Industry Use Cases

### Manufacturing

- **CPwE Architecture:** Converged Plantwide Ethernet, IACS, zones, IDMZ
- **Protocols:** EtherNet/IP, PROFINET, Modbus/TCP
- **Security:** Defense-in-depth, NAT, patching, anomaly detection

### Oil & Gas

- **Value Chain:** Upstream, midstream, downstream
- **Use Cases:** Connected oil field, pipeline, refinery
- **Security:** Asset inventory, remote access, patching, anomaly detection

### Utilities (Smart Grid)

- **GridBlocks Model:** 11-tiered, substation automation (IEC 61850, GOOSE, SV)
- **Resiliency:** PRP, HSR, MPLS-TP
- **Security:** NERC CIP, access control, data integrity

### Smart Cities

- **Architecture:** Street, city, data center, services
- **Use Cases:** Lighting, parking, traffic, environment
- **Security:** Device authentication, network encryption, privacy

### Transportation

- **V2X:** DSRC/WAVE, C-V2X, 802.11p
- **Fleet Management:** Telematics, diagnostics, Wi-Fi
- **Security:** Authentication, encryption, MACsec

### Public Safety

- **Mission Continuum:** Fixed, mobile, citizen-to-authority
- **Use Cases:** Emergency response, school bus safety, video analytics

---

## Industrial Automation Fundamentals

- **PLC:** Real-time control, scan cycle (input, logic, output, housekeeping)
- **SCADA:** Supervisory control, RTUs, PLCs, HMI, comms
- **LabVIEW:** Graphical programming, DAQ, OPC, high-speed measurement

---

## Exam Preparation Tips

1. **Active Recall:** Summarize each section in your own words.
2. **Draw Diagrams:** Practice from memory (IoT stacks, Purdue, protocol flows).
3. **Comparison Tables:** For protocols, architectures, security frameworks.
4. **Flashcards:** Acronyms, protocol features, key terms.
5. **Scenario Practice:** Apply concepts to real-world problems.
6. **Prioritize:** Focus on high-yield topics (security, architectures, protocols).
7. **Mock Questions:** Write and answer your own exam questions.

---

**Good luck!** Use this guide as a roadmap, and refer to your PDFs and slides for deeper details and diagrams. If you need a focused summary on any specific topic, just ask!
