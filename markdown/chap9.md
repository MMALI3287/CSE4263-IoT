# Chapter 9: Manufacturing

## Introduction

Business imperatives are evolving across industries, and manufacturing is no exception. While controlling costs and improving efficiency remain critical, the focus is shifting toward innovation and enhanced business models. This chapter explores the disruptive forces of digitization and IoT in manufacturing and innovative architectures for digitizing factories and connecting machines.

### Chapter Sections

- **Introduction to Connected Manufacturing**: Technologies driving digital disruption, strategies for connected factories, and business benefits.
- **Converged Factory Architecture**: The Converged Plantwide Ethernet (CPwE) architecture by Cisco and Rockwell Automation.
- **Industrial Automation Control Protocols**: Networking and control protocols like EtherNet/IP, PROFINET, and Modbus/TCP.
- **Connected Factory Security**: Key security considerations and design methodologies.
- **Edge Computing in the Connected Factory**: Implementing edge computing for improved data management and visibility.

---

## Introduction to Connected Manufacturing

### Key Challenges

A survey of over 400 manufacturing leaders identified the following top challenges:

- Meeting customer delivery dates
- Responding to unforeseen events
- Cost of poor quality and scrap
- Energy and maintenance costs
- Downtime and labor costs
- Material costs and production planning
- Rapid production adjustments and new product introduction cycles

### Aging Infrastructure

- The average age of automation infrastructure in the U.S. is the highest since 1938.
- 75% of U.S. plants are over 20 years old.
- 90% of the 60 million machines in factories worldwide are not connected, with most being over 15 years old.

### IoT-Driven Technologies

- **Data-Driven Manufacturing**: Real-time quality control, improved equipment effectiveness, and reduced downtime.
- **OT and IT Convergence**: Unified operational and information technology infrastructure.
- **Cost-Effective Connectivity**: Scaled, automated, and platform-based machine connectivity.
- **Machines as a Service (MaaS)**: Zero-touch deployment and remote monitoring.

### IoT Strategy for Connected Manufacturing

- **Software Ubiquity**: Transitioning physical controls to software for cost-effective management.
- **AI and Self-Diagnosis**: Machines self-diagnose and repair issues through software updates.
- **Real-Time Data Collection**: Full visibility into KPIs across the plant floor, enterprise, and supply chain.

---

## Summary

Manufacturers are leveraging IoT and digital transformation to modernize aging facilities, improve efficiency, and drive innovation. By connecting machines and adopting advanced architectures like CPwE, manufacturers can achieve significant business improvements.

---

## Converged Factory Architecture

### CPwE Overview

The Converged Plantwide Ethernet (CPwE) reference model, co-developed by Cisco and Rockwell Automation, focuses on the transport of EtherNet/IP. Key components include:

- **Cell/Area Zone**: Contains IACS devices (Levels 0–2) like HMIs and controllers.
- **Industrial Zone**: Supports IP routing for Level 3 applications.
- **Demilitarized Zone (DMZ)**: Manages secure traffic flows between industrial and enterprise zones.

### Resilient Network Design

Key capabilities for resilient IACS networks:

- **Availability**: Redundant physical paths for critical operations.
- **Predictable Performance**: Reliable, real-time traffic requirements.
- **Fast Network Reconvergence**: Restoration times under 100 ms.
- **Industrial Protocol Support**: Compatibility with industrial application protocols.

### Resilient Ethernet Protocol (REP)

- Achieves sub-50 ms convergence times in ring topologies.
- Supports unlimited nodes per segment, unlike traditional STP.
- Utilizes a master node for segment control and failure notifications.

---

## Connected Factory Security

### Holistic Security Approach

A "defense-in-depth" strategy addresses internal and external threats with multiple layers of defense:

- **Control System Engineers**: Device hardening, network segmentation, and application authentication.
- **IT Collaboration**: Zone-based firewalls and policy-driven access control.

### Industrial DMZ

The IDMZ enforces data security policies between trusted (industrial) and untrusted (enterprise) networks. Key principles:

- All IACS traffic terminates in the IDMZ.
- Centralized policy for network access.
- Streamlined device onboarding and guest portal services.

---

## Edge Computing in the Connected Factory

### Challenges with Traditional Approaches

- PCs on the plant floor require frequent maintenance and are prone to hardware failures.
- Difficulties in aggregating and analyzing data effectively.

### Edge Computing Solutions

- **Ruggedized Edge Appliances**: Combine switching, routing, and security features.
- **Standard Protocols**: Support for MTConnect, OPC UA, and PackML.
- **Streaming Analytics**: Refines data on the plant floor before transmitting to the cloud.

### Business Benefits

- Reduced costs for secure machine data collection.
- Optimized network resources and bandwidth.
- Enhanced visibility and actionable insights through OEE analytics tools.

---

This chapter provides a comprehensive overview of the transformative impact of IoT and digital technologies on manufacturing, emphasizing the importance of connected machines, resilient architectures, and secure, efficient data management.
