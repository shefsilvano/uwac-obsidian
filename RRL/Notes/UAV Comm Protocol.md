## Communication Layer 



# Basis for Ad hoc networking 
[[Wireless Ad Hoc Network of MANET_ VANET_ FANET and SANET A Review.pdf]]


[[Towards_Enhancement_of_Network_Communication_Architectures_and_Routing_Protocols_for_FANETs_A_Survey.pdf]]

### Problems in WANET 
WANET (Wireless Ad hoc network) - MANET, FANET, VANET, SANET 
> ([[Wireless Ad Hoc Network of MANET_ VANET_ FANET and SANET A Review.pdf#page=1&selection=391,19,399,6&color=yellow|it is not easy to develop a MANET for devices that move dynamically in the network [14].]])
> it is not easy to develop a MANET for devices that move dynamically in the network [14]. 


**Definition of Mobility models**
Mobility models in ad hoc networks describe ==how mobile nodes change their location, speed, and direction over time to simulate realistic movement in network evaluations==

> ([[Wireless Ad Hoc Network of MANET_ VANET_ FANET and SANET A Review.pdf#page=5&annotation=494R|p.5]])
> The ultimate purpose of mobility models is to demonstrate the direction, acceleration,  and speed of a node

> ([[Wireless Ad Hoc Network of MANET_ VANET_ FANET and SANET A Review.pdf#page=5&annotation=506R| Mobility discussion, p.5]])
> Therefore,  it is  crucial  to  identify  a  specific mobility model to ensure real-world deployment.


**On routing protocols**
> ([[Wireless Ad Hoc Network of MANET_ VANET_ FANET and SANET A Review.pdf#page=4&selection=654,16,659,35&color=yellow|Besides, it is also uncertain where these routing protocols may have been developed to be reliable on either low or high mobility nodes.]])
> Besides, ==it is also uncertain where these routing protocols may have been developed to be reliable on either low or high mobility nodes==. 



### [[FANET]]
> ([[Wireless Ad Hoc Network of MANET_ VANET_ FANET and SANET A Review.pdf#page=3&selection=67,0,119,14&color=yellow|p.3]])
> ==FANET is a special class of MANET that resembles VANET [39].== In other words, there is also the commonality of mobility in FANET, as it is in MANET and VANET [40]. FANET is a type of network that consists of mobile agents called ==micro aerial vehicles (MAVs) [41]==. These flying agents make up a group of small MAVs connected on an ad hoc basis to communicate for the required purposes. ==The existence of these flying agents typically results in the frequent changes of FANET’s network topology [42].== Figure 3 depicts a FANET architecture.





### Comm Protocol

**Intra and Inter-cluster communication**
Intra cluster - within the cluster comms protocol 
Inter - with other clusters 

## ESP-WIFI-MESH and painlessMesh 

ESP WIFI MESH - https://www.espressif.com/en/products/sdks/esp-wifi-mesh/overview

https://docs.espressif.com/projects/esp-idf/en/stable/esp32/api-guides/esp-wifi-mesh.html

![[Pasted image 20261127111706.png]]


> ([[Implementation_of_a_WiFi-based_V2V-V2I_Communication_Unit_for_Low_Speed_Vehicles.pdf#page=2&annotation=112R|Implementation_of_a_WiFi-based_V2V-V2I_Communication_Unit_for_Low_Speed_Vehicles, p.2]])
> It provides a ==self-forming and self-healing network== with ease of deployment. 


painlessMesh Library - [Github link ](https://github.com/gmag11/painlessMesh)

## ESP-NOW 

https://www.espressif.com/en/solutions/low-power-solutions/esp-now

> ([[Implementation_of_a_WiFi-based_V2V-V2I_Communication_Unit_for_Low_Speed_Vehicles.pdf#page=2&selection=93,20,95,14&color=yellow|Implementation_of_a_WiFi-based_V2V-V2I_Communication_Unit_for_Low_Speed_Vehicles, p.2]])
> The ESP-NOW protocol provides a fast, ==connection-less WiFi communication involving short packet transmission.==
* no handshake required but **requires pairing first** 

### [[Implementation_of_a_WiFi-based_V2V-V2I_Communication_Unit_for_Low_Speed_Vehicles.pdf]]
**combined both ESP-WIFI-MESH and ESP-NOW on their use cases.** 

In connection to VANETS, 
[[Wireless Ad Hoc Network of MANET_ VANET_ FANET and SANET A Review.pdf#page=2&selection=339,27,346,24&color=yellow|Due to its dynamic nature, the lack of realistic models and the capability to support an increasing number of vehicles has been an imperative topic for many researchers to discover.]]


- ESP-MESH
	Other vehicles outside the range of the RSU (with connection) can connect via the vehicle already inside the range 
	- ![[Pasted image 20261126113954.png]]
- ESP NOW
	When there are no detected RSUs, ESP-NOW runs to directly communication with another vehicle (with the prototype comm board) 
	
	![[Pasted image 20261126114222.png]]
		
![[Pasted image 20261126114538.png]]
Algorithm of the ESP-NOW + ESP-MESH implementation



# [[WiFi_networks_on_drones.pdf | Wifi Networks on Drones, Guillen Perez 2016]]

Experimented on different drone height under LOS conditions with consideration of different models for theoretical maximum 
## Key Findings
* Infra mode performs better in terms of data rate and coverage 
* Ad hoc operational mode is more responsive and energy-efficient

# [[Rotta 2024]]
 >([[A_Modular_Communication_Architecture_for_Adaptive_UAV_Swarms.pdf#page=3&annotation=200R|p.3]])
> The speed of the vehicles is limited by safe braking distances, which in turn depend on the communication range and telemetry broadcast rate

* Offloading communication load with different links of radio. Used UWB transceivers and 2.4 GHz WiFi. 
