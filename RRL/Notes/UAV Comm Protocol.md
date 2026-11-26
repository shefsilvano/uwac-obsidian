## Communication Layer 



# Basis for Ad hoc networking 
[[Wireless Ad Hoc Network of MANET_ VANET_ FANET and SANET A Review.pdf]]



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

Experimented on different drone height under LOS conditions with consideration of different models for theoretical maximum distance/ coverage/
## Key Findings
* Infra mode performs better in terms of data rate and coverage 
* Ad hoc operational mode is more responsive and energy-efficient
* 
> ([[WiFi_networks_on_drones.pdf#page=5&selection=524,36,555,43&color=yellow|WiFi_networks_on_drones, p.5]])
> lease also note that the attained values are far from those measured under controlled conditions, so the drone motion, a **possible radio interference caused by the drone’s chassis, or the environmental changing conditions seem to have a remarkable impact on the system performance**



> ([[WiFi_networks_on_drones.pdf#page=3&selection=128,50,130,19&color=yellow|The total weight of the board, the battery, and the antennas is approximately 340 g]])
> The <mark style="background:#d3f8b6">total weight </mark>of the board, the battery, and the antennas is approximately <mark style="background:#d3f8b6">340 g</mark>

>[!important] Component
> * Idea-Fly IFLY-4S drone with 700 g of payload
> * Intel Galileo dev board 
> *  Intel Dual-band Wireless AC 7260
> * 10400 mAh battery
> * 2 5 dBi Omnidirectional Antennas

# Methodology

> [!PDF|important] [[WiFi_networks_on_drones.pdf#page=3&selection=134,4,151,23&color=important|p.3]]
> . We assumed an open-air scenario and selected two radio propagation models: Free Space (or Friis) model [20] and the Wireless World Initiative New Radio (WINNER) D1 model [21].


### Infrastructure Mode 
> ([[WiFi_networks_on_drones.pdf#page=3&selection=185,0,189,46&color=yellow|p.3]])
> This mode deploys a network within the coverage area of a central device (the access point, AP), ==which interconnects all nodes composing the system and acts as a gateway towards an external network (e.g., Internet).== 


### Ad-hoc Mode 

> ([[WiFi_networks_on_drones.pdf#page=3&selection=227,1,256,19&color=yellow|p.3]])
> n this case, each node simultaneously assumes both client/host and router tasks, ==hence network nodes periodically scan for retrieving information about their neighboring nodes.== 

* dynamic routing that eliminates the coverage constraint 
* BATMAN ad hoc routing protocol which has superior performance under heavy traffic loads [23]

>[!note] Important Tools for Metrics 
>* iPerf3 tool to obtain network metrics 
>	* Maximum achievable bandwidth 
>	* Throughput
>	* Packet loss 
>	* packet delay
>
>* Constant Bit Rate transmissions ([[WiFi_networks_on_drones.pdf#page=3&selection=359,0,379,13&color=red|CBR]]) with 30 sec durations 
>* Field measurements with CBR, two different heights, and energy-efficiency through test-bench measurement, DAQ and Matlab

### Results 
> ([[WiFi_networks_on_drones.pdf#page=6&annotation=80R|WiFi_networks_on_drones, p.6]])
> Accordingly, the cards are self- configured to work in a different version of the standard as a function of the link quality, thus employing different modulations, which in turn determines the maximum link

