---
Author/s: Ganesh, Gopalasamy, Sai Shibu N B
Title: Architecture for Drone Assisted Emergency Ad-hoc Network for Disaster Rescue Operations
Publication: COMSNETS
Category: "[[Architecture]]"
Summary: Proposed UbiQNet architecture that establishes the use of two WiFi-based communication protocol to form a mesh network.
tags:
Year: "2021"
---


[[Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations.pdf]]


# Essence
- Principal paper of the project? 
- ESP32-based SoC that runs the [[Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations.pdf#search=A. UbiQNet- Ubiquitous Network for Emergency Communication|UbiQNet]] with Lithium-ion battery on top of the drone 
- Walang network testing, more on proposal of an architecture or system only

## Methodology  
>[!note] Assumptions 
>* Users and first responders have mobile devices with WiFi capabilities
>* Portable computer must be used for messaging 

>[!note] UbiQNet - Ubiquitous Network for Emergency Communications 
>* Composes of an<font color="#00b050"> ESP32-based SOC</font>, drone, mobile devices, and portable computer 
>* ESP32 Modes - Station (For UAV control) and AP (for comms) 
>* <font color="#00b050">Communication of nodes is through REST API calls </font>
>* Portable computer for communication and organizing database (store info) of the victims

>[!note] Communication Protocol 
> ESP Wifi Mesh Protocols 
> * 802.11 LR -  surveillance (high range, less BW, more power consumption)
> * 802.11 b - for UbiQnet  (less range, more BW, less power consumption)
> * Add details about ESP MESH network



* UAV Return to Home function 


