# IoT Exam Study Guide: Comprehensive Preparation

This guide is designed to help you prepare for your IoT exam by synthesizing key concepts, architectures, protocols, security practices, and industry applications. Use it alongside your PDFs and lecture notes for a deep understanding.

## Table of Contents

- [IoT Exam Study Guide: Comprehensive Preparation](#iot-exam-study-guide-comprehensive-preparation)
  - [Table of Contents](#table-of-contents)
  - [1. Core IoT Concepts](#1-core-iot-concepts)
    - [1.1. Definition \& Scope](#11-definition--scope)
    - [1.2. IoT Architectures](#12-iot-architectures)
  - [2. Smart Objects \& Connectivity](#2-smart-objects--connectivity)
    - [2.1. Sensors \& Actuators](#21-sensors--actuators)
    - [2.2. Connectivity Protocols](#22-connectivity-protocols)
  - [3. IP Networking in IoT](#3-ip-networking-in-iot)
    - [3.1. 6LoWPAN \& RPL](#31-6lowpan--rpl)
  - [4. IoT Application Protocols](#4-iot-application-protocols)
    - [4.1. CoAP \& MQTT](#41-coap--mqtt)
  - [5. Data Management \& Analytics](#5-data-management--analytics)
    - [5.1. Big Data \& Machine Learning](#51-big-data--machine-learning)
  - [6. IoT Security](#6-iot-security)
    - [6.1. Challenges \& Best Practices](#61-challenges--best-practices)
  - [7. Industry Use Cases](#7-industry-use-cases)
    - [7.1. Manufacturing, Utilities, Smart Cities](#71-manufacturing-utilities-smart-cities)
  - [8. Exam Preparation Tips](#8-exam-preparation-tips)

---

## 1. Core IoT Concepts

### 1.1. Definition & Scope

- **IoT Definition**: Interconnected physical objects ("things") with sensing, processing, and communication capabilities.
- **Key Drivers**: Scale (billions of devices), constrained resources, real-time data, security/privacy, legacy integration.
- **IT vs. OT**: IT prioritizes CIA (Confidentiality, Integrity, Availability); OT focuses on AIC (Availability, Integrity, Safety).

### 1.2. IoT Architectures

- **IoTWF 7-Layer Model**: Physical devices, connectivity, edge/fog, data accumulation, data abstraction, applications, collaboration.
- **Purdue Model**: Levels 0–5 (field devices to enterprise), DMZ between IT/OT.
- **Simplified 3-Layer Stack**: Things, network, applications/analytics.

## 2. Smart Objects & Connectivity

### 2.1. Sensors & Actuators

- **Sensors**: Detect physical quantities (e.g., temperature, pressure).
- **Actuators**: Perform actions (e.g., motors, valves).
- **MEMS**: Micro-Electro-Mechanical Systems for miniaturized devices.

### 2.2. Connectivity Protocols

| **Protocol** | **Range** | **Power** | **Data Rate** | **Topology**  |
| ------------ | --------- | --------- | ------------- | ------------- |
| **ZigBee**   | 10–100 m  | Low       | 250 kbps      | Mesh          |
| **LoRaWAN**  | 15–30 km  | Very Low  | 0.3–50 kbps   | Star-of-Stars |
| **NB-IoT**   | Cellular  | Low       | 20–100 kbps   | Star          |

## 3. IP Networking in IoT

### 3.1. 6LoWPAN & RPL

- **6LoWPAN**: IPv6 over low-power wireless (header compression, fragmentation).
- **RPL**: Routing Protocol for LLNs (DODAGs, ETX metric).

## 4. IoT Application Protocols

### 4.1. CoAP & MQTT

| **Feature**   | **CoAP** | **MQTT** |
| ------------- | -------- | -------- |
| **Transport** | UDP      | TCP      |
| **Model**     | RESTful  | Pub/Sub  |
| **Security**  | DTLS     | TLS      |

## 5. Data Management & Analytics

### 5.1. Big Data & Machine Learning

- **3 Vs**: Volume, Velocity, Variety.
- **Tools**: Hadoop, Spark, NoSQL databases.
- **ML Applications**: Predictive maintenance, anomaly detection.

## 6. IoT Security

### 6.1. Challenges & Best Practices

- **Challenges**: Legacy systems, constrained devices, data privacy.
- **Best Practices**: Device security (secure boot), network security (segmentation), risk analysis (OCTAVE, FAIR).

## 7. Industry Use Cases

### 7.1. Manufacturing, Utilities, Smart Cities

- **Manufacturing**: CPwE architecture, EtherNet/IP, PROFINET.
- **Utilities**: GridBlocks model, IEC 61850, PRP/HSR.
- **Smart Cities**: IoT for lighting, parking, traffic.

## 8. Exam Preparation Tips

1. **Active Recall**: Summarize concepts in your own words.
2. **Diagrams**: Redraw architectures and protocols.
3. **Flashcards**: Acronyms and definitions.
4. **Scenario Questions**: Apply concepts to real-world problems.
