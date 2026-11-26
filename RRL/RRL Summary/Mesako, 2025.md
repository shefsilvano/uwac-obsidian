---
Title: "[[Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System.pdf]]"
Author/s: Mesako, Kumakura, Tajima, Zhang
Publication: Consumer Communication & Networking Conference (CCNC)
Category: "[[UAV Comm Protocol]]"
Summary: Proposed a combination of an ad hoc routing protocol (AODV) and SDN protocol (OpenFlow) with utilization of an SDN controller.
Year: "2025"
Bibtex: "@INPROCEEDINGS{10975949,\r

  \  author={Maesako, Keisuke and Kumakura, Ken and Tajima, Yusuke and Zhang, Liang},\r

  \  booktitle={2025 IEEE 22nd Consumer Communications & Networking Conference (CCNC)}, \r

  \  title={Field Trial of Drones with an Aerial Wireless Mesh Network Control System}, \r

  \  year={2025},\r

  \  volume={},\r

  \  number={},\r

  \  pages={1-7},\r

  \  keywords={Measurement;Wireless communication;Wireless mesh networks;Traffic control;Throughput;Routing;Routing protocols;Software defined networking;Optimization;Drones;aerial communication platform;aerial wireless mesh networks;software-defined networking;combinatorial optimization;drone networks;field trial},\r

  \  doi={10.1109/CCNC54725.2025.10975949}}"
---
[[Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System.pdf]]




	
# Essence 
Utilization of different routing algorithms through SDN controller to control overhead in the mesh, or the bandwidth of the network 

Allow the immediate re-routing and discovery of nodes when one leaves

~~May have conflict with the SDN controller as a common point of failure~~ 

Resolves the limitation of static route-based multihopping between nodes while being connected to the SDN  

The use of SDN makes routing 
# [[System Architecture]] 

![[Pasted image 20261125180240.png]]

Routing Control Process between the AODV and SDN 

[[Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System.pdf#page=2&selection=335,23,337,32&color=yellow|Switching Operations between SDN and AODV]]

![[Pasted image 20261125184428.png]]

# Methodology

> [!PDF|important] [[Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System.pdf#page=2&selection=109,38,116,10&color=important|Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System, p.2]]
>  Here, **the route distributed by the controller is used for data communication, and the route set by the ad hoc routing protocol is used only for the purpose of controller connection.**

SDN Controller - Data communication 
Ad hoc routing protocol (AODV) - for all nodes to reach the controller

>[!note] [[AODV]]  Ad hoc On-Demand Distance Vector routing protocol 
>*  reactive ad hoc routing that calculates routes only for the SD pairs
>* minimizes the volume of control packet traffic in comparison to OLSR 


>[!important] Components 
> * [[DJI Neo 2 Fly More Combo]] for field test 
> * Raspberry Pi 4 as SDN Switch 


### Communication 
> [!PDF|important] [[Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System.pdf#page=1&selection=433,0,437,54&color=important|Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System, p.1]]
> As mentioned in Section 1, SDN achieves flexible route control in a wireless mesh network. The prerequisite is that all nodes must be continuously connected to the controller

> ([[Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System.pdf#page=2&selection=18,0,22,10&color=yellow|Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System, p.2]])
> Therefore, **==nodes that are not directly connected to the ground gateway should connect to the controller via a multihop connection==**


### [[SDN-hosted routing algorithm]]

1. [[Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System.pdf#page=3&selection=97,0,97,24&color=yellow|Routing metric algorithm]]
2. [[Field_Trial_of_Drones_with_an_Aerial_Wireless_Mesh_Network_Control_System.pdf#page=3&selection=202,36,202,37&color=yellow|Combinatorial optimization algorithm]] 

