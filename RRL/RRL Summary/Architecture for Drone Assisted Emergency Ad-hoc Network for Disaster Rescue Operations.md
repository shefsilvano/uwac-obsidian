[[Architecture_for_Drone_Assisted_Emergency_Ad-hoc_Network_for_Disaster_Rescue_Operations.pdf]]



# Essence
- Principal paper of the project? 
- ESP32-based SoC that runs the <mark style="background:#affad1">UbiQNet</mark> with Lithium-ion battery on top of the drone 
- Walang network testing, more on proposal of an architecture or system only


# Key Findings
## Methodology  
>[!todo] Assumptions 
>* Users and first responders have mobile devices with WiFi capabilities
>* Portable computer must be used for messaging 

>[!todo] UbiQNet - Ubiquitous Network for Emergency Communications 
>* Composes of an<font color="#00b050"> ESP32-based SOC</font>, drone, mobile devices, and portable computer 
>* ESP32 Modes - Station (For UAV control) and AP (for comms) 
>* <font color="#00b050">Communication of nodes is through REST API calls </font>
>* Portable computer for communication and organizing database (store info) of the victims

>[!todo] Communication Protocol 
> ESP Wifi Mesh Protocols 
> * 802.11 LR -  surveillance (high range, less BW, more power consumption)
> * 802.11 b - for UbiQnet  (less range, more BW, less power consumption)
> * Add details about ESP MESH network



* UAV Return to Home function 


