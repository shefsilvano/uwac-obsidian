---
Author/s: Ganesh, Gopalasamy, Sai Shibu N B
Title: "[[Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations.pdf]]"
Publication: COMSNETS
Category: "[[System Architecture]]"
Summary: Proposed UbiQNet architecture that establishes the use of two WiFi-based communication protocol to form a mesh network.
tags:
Year: "2021"
---


[[Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations.pdf]]


# Essence
- Principal paper of the project? 
- ESP32-based SoC that runs the [[Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations.pdf#search=A. UbiQNet- Ubiquitous Network for Emergency Communication|UbiQNet]] with Lithium-ion battery on top of the drone 
- Walang network testing, more on proposal of an architecture or system only
### Problem Statement
> ([[Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations.pdf#page=3&selection=45,11,49,31&color=yellow|Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations, p.3]])
> It is because of these reasons that the ability to communicate directly with first responders during this time period, allowing one to share their location with those working in rescue will greatly increase the chance of being saved before the situation gets exacerbated.

* **"A communication portal"**
## Methodology  


> ([[Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations.pdf#page=2&annotation=101R|Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations, p.2]])
> this is eliminated in our architecture, where one of the nodes in the mesh network can be elected as the root node

### [[System Architecture]]

![[Pasted image 20261125154421.png]]
![[Pasted image 20261125144028.png|275]]

End users  - first responders (FR) and the victims/stranded people 



>[!note] Assumptions 
>* Users and first responders have mobile devices with WiFi capabilities
>* Portable computer must be used for messaging 

### Proponents  
1. SoC
2. UaV
3. Mobile device of the users/victims
4. Portable computer 

>[!important ] Components:
> * ESP32 SoC (32-bit dua-core LX6 processor, 448 KB ROM and 520 KB SRAM coupled with 16 KB SRAM in RTC) 
> * LiPo battery (for the ESP )
> * Drone 
>



>[!note] UbiQNet - Ubiquitous Network for Emergency Communications 
>* Composes of an<font color="#00b050"> ESP32-based SOC</font>, drone, mobile devices, and portable computer 
>* ESP32 Modes - Station (For UAV control and preprogramming) and AP/Soft AP (for comms) 
>* Combined  (AP-STA) - station connected to another access point
>* REST API calls accepted by the portable computer

>* Portable computer for communication and organizing database (store info) of the victims **in the FR side**

**UAV Preprogramming - setting waypoints to the drone and set return to home after operations** 

### Communication Workflow
>[!note] Communication Protocol 
> ESP Wifi Mesh Protocols 
> * 802.11 LR -  surveillance (high range, less BW, more power consumption)
> * **802.11 b - for UbiQnet  (less range, more BW, less power consumption)**
> * Add details about ESP MESH network

> [!PDF|yellow] [[Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations.pdf#page=5&selection=39,21,58,56&color=yellow|p.5]]
>  The maximum size of each node can be 16 elements and n can take up any value. The selection of which FR should this message reach is determined by the following scenarios. 
>  
>  • Case 1: Consider Figure 5, if the FR is a leaf node in the same intermediate node. Then, the victim contacts this FR. 
>  
>  • Case 2: Consider Figure 6, if there are no leaf nodes with FR, then the next closest leaf node with FR is identified. Then, the FR on this network is contacted by the victim.

**Leaf Node** -  node where the FR is connected or in close proximity 

>[!question] Meshing terms and concepts
>* Root node selection  
>* Parent node selection
>* Power-on Reset 


# Verdict 
* Lacks results and metrics on whether how the architecture performed 
* Proposal for architecture but really without specifying or delving into the details of meshing in relation to root/parent/ node selection ( I think this is outside the scope/objective of the study)
