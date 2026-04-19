# Hybrid-Cloud-Visibility-Sentinel-Azure-Arc
Centralising hybrid security telemetry by integrating on-premises infrastructure with Microsoft Sentinel via Azure Arc for unified visiblity.

## 📌 Project Overview
This project demonstrates the implementation of a hybrid security monitoring solution. By integrating on-premises infrastructure with **Microsoft Sentinel** via **Azure Arc**, I eliminated visibility blind spots and created a unified "Single Pane of Glass" for security telemetry.

The goal was to bridge the gap between local hardware and cloud-native SIEM capabilities, ensuring all security events are centralised to aid monitoring and analysis.

---

## 🛠️ Technical Stack
* **SIEM:** Microsoft Sentinel
* **Hybrid Management:** Azure Arc
* **Telemetry Repository:** Log Analytics Workspace (LAW)
* **Log Ingestion:** Azure Monitor Agent (AMA)
* **Configuration:** Data Collection Rules (DCR)

---

## 🚀 Implementation Roadmap

### 1. Infrastructure Foundation
* Created a dedicated **Resource Group** and **Log Analytics Workspace** to serve as the central repository for all security telemetry.
* Initialised **Microsoft Sentinel** on the workspace to enable advanced analytics and incident management capabilities.

### 2. Machine Onboarding (The Hybrid Bridge)
* Successfully onboarded a local host machine to **Azure Arc**.
* This step allowed the local infrastructure to be managed and monitored as a native Azure resource.

### 3. Log Ingestion & Configuration
* Configured **Data Collection Rules (DCR)** to define exactly which telemetry should be captured.
* Set up the **Windows Security Events** connector via the **Azure Monitor Agent (AMA)** to stream real-time logs into Sentinel.

---

## 📂 Repository Structure
* **[/Architecture](./Architecture/)**: Final environment state and Azure Arc connectivity status.
* **[/Configuration](./Configuration/)**: Data Connector settings, Redacted DCR mapping, and Log ingestion verification.
* **[/Documentation](./Documentation/)**: Step-by-step onboarding documentation and PowerShell execution logs.

---

## 🏆 Key Achievements
* **Hybrid Visibility & Risk Mitigation:** Eliminated security blind spots by bridging isolated on-premises assets with cloud-native monitoring, creating a single pane of glass for all security telemetry.
* **Operational Excellence and Audit Readiness:** Streamlined security oversight by centralising hybrid logs into a single console, establishing a veifiable audit trail for non-Azure infrastructure.
