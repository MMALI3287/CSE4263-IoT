# Chapter 8: Securing IoT

## Introduction

It is often said that if World War III breaks out, it will be fought in cyberspace. As IoT brings more systems together under the umbrella of network connectivity, security has never been more important. From the electrical grid system that powers our world to the systems that keep airplanes flying, security of networks, devices, and applications is foundational for modern communication systems. However, providing security in such a world is not easy.

Security is one of the few technology disciplines that must operate against external forces continually working against desired outcomes. These forces leverage both traditional technology and non-technical methods (e.g., physical security, operational processes) to meet their goals. With so many potential attack vectors, information and cybersecurity is a challenging but critical topic for technology vendors, enterprises, and service providers alike.

## IT vs. OT Security

### Key Differences

- **IT Environments**: Have faced active attacks and threats for decades, with well-documented incidents and lessons learned.
- **OT Environments**: Traditionally siloed with limited network connections, resulting in fewer documented incidents and learning opportunities. In OT, security often overlaps with safety, incorporating equipment and personnel safety recommendations.

### Focus of This Chapter

This chapter focuses on the core principles of securing OT environments, touching on IT security elements fundamental to OT security. It includes:

- A historical perspective of OT security.
- Common challenges in OT security.
- Key differences between IT and OT security practices.
- Formal risk analysis structures (e.g., OCTAVE and FAIR).
- A phased approach to introducing modern IT network security into legacy industrial environments.

## Historical Perspective of OT Security

### Key Incidents

- **Stuxnet Malware**: Damaged uranium enrichment systems in Iran.
- **German Smelter Incident**: Damaged a furnace due to a cyberattack.
- **Maroochy Shire Sewage Attack (2000)**: Released 800,000 liters of sewage into waterways.
- **Kyiv Oblenergo Power Outage (2015)**: Caused hours-long outages and degraded service for thousands.

### Challenges

- Legacy protocols in IoT environments often lack security considerations.
- Attackers now have access to tools that make launching attacks easier, increasing the frequency and threat level.

## Common Challenges in OT Security

### Erosion of Network Architecture

- Initial designs often assumed physical separation ensured safety.
- Over time, ad hoc updates and changes eroded original security designs.

### Pervasive Legacy Systems

- Many operational systems are outdated and lack modern security patches.
- Communication infrastructure often relies on decades-old protocols.

### Insecure Operational Protocols

- **Modbus**: Lacks endpoint authentication and validation.
- **DNP3**: Emphasizes reliable delivery but lacks trust mechanisms.
- **ICCP**: Initially lacked authentication and encryption.
- **OPC**: Dependent on vulnerable Windows platforms.
- **IEC Protocols**: Known security deficiencies, such as clear-text passwords and unsigned firmware.

### Device Insecurity

- OT systems have not undergone the same rigorous security testing as IT systems.
- Vendors often lag in security practices and cooperation with researchers.

### Dependence on External Vendors

- Vendor access to critical systems is often required for maintenance, creating potential security risks.

### Security Knowledge Gap

- Industrial environments often lack security-focused human resources.
- Workforce aging and rapid technology changes exacerbate the gap.

## Formal Risk Analysis Structures

### OCTAVE (Operationally Critical Threat, Asset, and Vulnerability Evaluation)

- Focuses on lightweight, less burdensome processes.
- Steps include establishing risk criteria, profiling assets, identifying threats, and applying mitigations.

### FAIR (Factor Analysis of Information Risk)

- Emphasizes measurable, quantifiable metrics.
- Defines risk as the probable frequency and magnitude of loss.
- Focuses on six forms of loss: productivity, replacement, response, fines, competitive advantage, and reputation.

## Phased Application of Security

### Secured Network Infrastructure and Assets

1. **Analyze and Secure Network Design**: Segment functions into zones and secure communication crossing boundaries.
2. **Perform Network Discovery**: Map physical connections and identify communication paths.
3. **Secure Connectivity**: Apply access control policies and encrypted communications (e.g., VPNs).

### Deploying Dedicated Security Appliances

- Use deep packet inspection (DPI) technologies for visibility and threat detection.
- Deploy firewalls and intrusion prevention systems (IPS) to manage access and ensure safety.

### Higher-Order Policy Convergence

- Coordinate IT and OT security practices.
- Implement network security monitoring (NSM) to detect and investigate intrusions.

## Summary

Modern industries must modernize securely. Increasing connectivity among legacy OT assets demands strong security measures to ensure operational efficiency and safety.
