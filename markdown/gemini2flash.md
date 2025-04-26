# IoT Exam Study Guide - v2.0

## 1. Introduction

This README provides a super-detailed structure for studying for your IoT exam, focusing on practical application, comparison, and memorization techniques. Use in conjunction with:

- "IoT Fundamentals" textbook (Hanes et al.)
- Provided powerpoint slide decks (Dr Syed Mustafa, HKBKCE)

Remember to understand the key takeaways for each topic and how the different topics covered are related.

## 2. Core Concepts & Architectures

### 2.1. Defining the Internet of Things

- **Definition**: Networked interconnection of physical objects ("things"), enabling data exchange and control without direct human intervention.
- **Beyond Definition**:
  - Envision a future where everything, from tractors to teacups, is interconnected.
  - Connecting the previously unconnected: Connecting devices to computer networks so that they can communicate and interact with people and objects (pg. 3 of "IoT Fundamentals")
- **Key Enablers:** Embedded systems, sensors, wireless communication, cloud computing, data analytics.
- **Distinguishing IoT from:**
  - **Digitization**: IoE (Internet of Everything) has been replaced by Digitization and encompasses connection of "things" with the data they generate & the business insights that result. In most contexts, duality is fine, but there are key differences to be aware of. IoT is subset of IoE and Digitization.

### 2.2. Key Architectural Concepts

- **Emphasis on layers**
- **3-Layer Architecture:**
  - **Layer 1: Things**: Sensors and Actuators layer
  - **Layer 2: Communications Network Layer** Access Network Sublayer, Gateways and Backhaul Sublayer, Network Transport Sublayer, IoT Network Management Sublayer
  - **Layer 3: Applications and Analytics Layer** Analytics Versus Control Applications, Data Versus Network Analytics, Data Analytics Versus Business Benefits, Smart Services
- **IoTWF (IoT World Forum) 7-Layer Architecture:**
  - How the layers operate and interact
- **Purdue Model for Control Hierarchy**
- Layered and well-defined structure

### 2.3 Challenges to loT and IT/OT convergence

- The scale is typically greater with IOT networks. An example is one large electrical utility in Asia recently began deploying IPv6-based smart meters on its electrical grid (p.40).
- Security (p.40)
- Privacy (p.40)
- Big data and data analytics (p.40)
- Interoperability

## 3. Network Technologies, Protocols and Layer by Layer Explanations

### 3.1 Layer 1: Physical Devices and Controllers

- Sensors: Types of sensors based on various parameters like whether or not they are connected.
- Actuators: Responsible for directly initiating a physical action. They are what is typically "controlled" as a result of IoT implementation.
- MEMS: Micro-Electro-Mechanical Systems

### 3.2. Layer 2: Connectivity (Communications Network Layer)

- **Access Network Sublayer**
  - WPAN
  - WHAN
  - WFAN
  - WLAN
- **Gateways and Backhaul Sublayer**

- **Network Transport Sublayer**

- **IOT Network Management Sublayer**

### 3.2.1 IoT Data-Link Layer Technologies

For each technology, know:

- **Standardization**: IEEE, IETF, 3GPP, Wi-SUN Alliance
- **Frequencies**
- **Reach**
- **Power**
- **Physical and MAC Layer operation**
- **Data Rates**
- **Topologies supported**
- **Application & Integration Considerations**
- **Security Features**
- **Competitive Technologies**

This includes in depth study for:

- IEEE 802.15.4.
- IEEE 802.11 ah
- IEEE 802.15.4g/e.
- LoRaWAN.
- IEEE 1901.2a (NB-PLC)
- Cellular IOT (NB-IOT, LTE-M).

### 3.2.2 Key Mesh Networking parameters for IOT networks

- A mesh topology helps cope with low transmit power, searching to reach a greater overall distance, and coverage by having intermediate nodes relaying traffic to other nodes.

### 3.3 Power Considerations for each Connectivity Technology

- What is power class (short, medium, and long range capabilities)?
- Power efficient sleep protocols: IEEE 802.11 power save specifications
- What battery topologies can be implemented for each reach?

## 4. IP as the IoT Network Layer (and related sublayers)

### 4.1 The Business Case for IP

- The Layer 3 and 4 advantages of selecting IP include:
  -Open, standards-based nature
  -Ubiquity
  -Scalability
  -Manageability and Security
  -Resiliency.

### 4.2 IP and 6LoWPAN

- 6LoWPAN (IPv6 over Low Power Wireless Personal Area Networks) enables IPv6 over IEEE 802.15.4. How data packets look.
- Low power is often a trade for security, performance, or other metrics. How do you ensure you have selected the right configurations to cope with these metrics, as well.

### 4.3 Transport

- Delineate the differences in transport layer
- TCP vs UDP for IOT

### 4.4 IEEE 802.11 and wireless

\*What is the difference, performance, throughput? How it is being used.

## 7. IoT Application Protocols

- **The transport layer**: the selection of a protocol for transport layer
- **UDP**: explain the functions in terms of use
- **TCP**: explain the function in terms of use
- **Adapt legacy protocols**: look over SCADA transport protocols (DNP3) and their implementation
- **Web Services and protocol**:
  - COAP: The architecture of the protocols. Is a great way to look a generic approach from that protocols.
  - MQTT: The architecture of it, how works is important.
  - How they impact in certain sectors is important too (COAP Vs MQTT)

## 8. Data and Analytics for IoT

- Data generated and analysed: in that framework.
- Data needs (are processed).
  - Bigdata analitics: Is an overview for that process (used to correlate between data and intelligence
  - Data needs to be managed
- Various type of data and Analytics (Structured Vs unstructured data)
  - Network data: that information must be used
    •The technology must be implemented properly, the types of information of the internet, also information should be high quality and that architecture need to be used.

## 9. Securing IoT

- OT and IT security \* What are their practices
- How the systems vary.
- New risk of information is created that means they need for that is the framework and the analysis is there
- New types of analytics there that are made which should know how it is implied to there is all types of the above requirements
  •The systems must be good and have the highest quality to support that

## 10. IoT in Industry - 7 Main Sectors

• manufacturing (What changes occurs on it and what technology to use for that sector - (how they change those equipment) is very important to remember
• Oil and Gas (similar to manufacture sector, how they need to work it) that one for good information - What key drivers are going to affect its

## 11. Additional Material for Manufacturing

### 11.1. How can all this be accomplished by

*Using all data types in the environment.
*Different protocols with various technology
\*Various components of a correct computer.
(and give some key information of data)

---

## 12. Exam Preparation: Strategies and Tips

- Create your set of flashcards, protocols (with descriptions), protocols about their functions
- Give some memorization technique to remember
- Repeat: that is most important
- Practice tests
