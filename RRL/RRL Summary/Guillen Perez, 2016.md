---
Title: "[[WiFi_networks_on_drones.pdf]]"
Author/s: Guillen-Perez, Sanchez-Ibarra, Cano, Sanchez-Aarnoutse, Garcia-Haro
Publication: ITU Kaleidoscope
Category:
Summary:
Reading Status:
Citation: 'A. Guillen-Perez, R. Sanchez-Iborra, M. -D. Cano, J. C. Sanchez-Aarnoutse and J. Garcia-Haro, "WiFi networks on drones," 2016 ITU Kaleidoscope: ICTs for a Sustainable World (ITU WT), Bangkok, Thailand, 2016, pp. 1-8, doi: 10.1109/ITU-WT.2016.7805730.'
Bibtex: "@INPROCEEDINGS{7805730,\r

  \  author={Guillen-Perez, Antonio and Sanchez-Iborra, Ramon and Cano, Maria-Dolores and Sanchez-Aarnoutse, Juan Carlos and Garcia-Haro, Joan},\r

  \  booktitle={2016 ITU Kaleidoscope: ICTs for a Sustainable World (ITU WT)}, \r

  \  title={WiFi networks on drones}, \r

  \  year={2016},\r

  \  volume={},\r

  \  number={},\r

  \  pages={1-8},\r

  \  keywords={IEEE 802.11 Standard;Ad hoc networks;Wireless communication;Drones;Routing;Aerial network;UAV;drones;WiFi;low altitude platform;network access},\r

  \  doi={10.1109/ITU-WT.2016.7805730}}"
---


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
