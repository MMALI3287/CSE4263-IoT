# Connecting Smart Objects in IoT

IoT devices, sensors, and actuators must be connected to share their data. This chapter reviews:
• Frequency bands used for IoT (especially unlicensed ISM and sub‑GHz bands) and their regulations.  
• Power consumption trade‑offs for powered versus battery‑operated nodes and how LPWA technologies address these needs.  
• Network topologies (star, mesh, peer‑to‑peer) and the role of constrained devices.  
• An overview of major IoT access technologies (IEEE 802.15.4 variants, NB‑PLC, IEEE 802.11ah, LoRaWAN, NB‑IoT, LTE variations).

## Frequency and Spectrum for IoT

• **Unlicensed ISM Bands:**  
 – 2.4 GHz (Wi‑Fi, Bluetooth, WPAN)  
 – Sub‑GHz bands (e.g., 169, 433, 868, 915 MHz) for better range and obstacle penetration

• **Regulatory Considerations:**  
 – Although unlicensed, these bands are regulated (transmit power, duty cycle, etc.)  
 – Regional differences: CEPT recommends 868 MHz for Europe; FCC governs 902–928 MHz in North America  
 – Some countries define additional bands (e.g., China’s 779–787 MHz)

## Power Consumption and LPWA

• **Node Types:**  
 – **Powered Nodes:** Have a direct power source but are limited by availability.  
 – **Battery-Powered Nodes:** Offer flexibility but require low power protocols; changing batteries frequently is unacceptable.

• **LPWA Technologies:**  
 – Designed for low throughput, long battery life, and extended link budgets  
 – Optimize bandwidth via narrow channels and duty cycle limits

## Network Topology

• **Star Topology:**  
 – Common in cellular, LPWA, and Bluetooth deployments; a central base station connects to all endpoints.

• **Mesh Topology:**  
 – Uses intermediate (relay) nodes to extend range  
 – Requires specialized routing protocols (e.g., RPL) and may use “mesh‑under” or “mesh‑over”

• **Peer‑to‑Peer:**  
 – Allows direct communication within range

## Constrained Devices and LLNs

• **Resource Limitations:**  
 – Defined by RFC 7228; nodes may lack full IP stacks  
 – Classifications:  
  • **Class 0:** Severely constrained (e.g., simple pushbutton)  
  • **Class 1:** Limited resources; can run optimized protocols (e.g., CoAP)  
  • **Class 2:** Sufficient resources for full IP stack

## Overview of IoT Access Technologies

• **IEEE 802.15.4 and Variants (802.15.4g/e):**  
 – Low‑cost, low‑data‑rate wireless PHY and MAC layers  
 – Used for home/building automation, industrial sensor networks  
 – Enhancements for security (AES), latency reduction, and mesh formations

• **NB‑PLC (IEEE 1901.2a):**  
 – Wired standard for Narrowband Power Line Communication  
 – Deployed for smart metering, distribution automation, and public lighting  
 – Supports meshed topologies over power lines with IP integration via 6LoWPAN

• **IEEE 802.11ah (Wi‑Fi HaLow):**  
 – A sub‑GHz extension of Wi‑Fi offering extended range and low power  
 – Ideal for IoT sensors and aggregating data in large cells

• **LoRaWAN:**  
 – An LPWA solution using Semtech’s LoRa modulation (chirp spread spectrum)  
 – Features a “star of stars” topology with gateways bridging endpoints to a network server  
 – Supports adaptive data rates via different spreading factors

• **NB‑IoT and LTE Variations:**  
 – Cellular LPWA technologies designed for massive, low‑throughput IoT deployments  
 – Evolved from LTE Cat 0/M to NB‑IoT with narrow channels (200 kHz) and extended coverage

## Summary Table of Access Technologies

| Characteristic  | IEEE 802.15.4    | IEEE 802.15.4g/e | IEEE 1901.2a | IEEE 802.11ah | LoRaWAN            | NB-IoT       |
| --------------- | ---------------- | ---------------- | ------------ | ------------- | ------------------ | ------------ |
| Connection Type | Wireless         | Wireless         | Wired        | Wireless      | Wireless           | Wireless     |
| Frequency Bands | 2.4 GHz, sub‑GHz | 2.4 GHz, sub‑GHz | Sub‑GHz      | Sub‑GHz       | Unlicensed sub‑GHz | Licensed     |
| Topology        | Star/Mesh        | Star/Mesh        | Star/Mesh    | Star          | Star of stars      | Star         |
| Range           | Medium           | Medium           | Medium       | Medium        | Long               | Long         |
| Data Rate       | Low              | Low              | Variable     | Low           | Low–moderate       | Low–moderate |
