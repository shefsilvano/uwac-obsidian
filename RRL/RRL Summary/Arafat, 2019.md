---
Author/s: Arafat & Moh
Title: Localization and Clustering Based on Swarm Intelligence in UAV Networks for Emergency Communications
Publication: IEEE Internet of Things Journal
Category: "[[Algorithms]]"
Summary: Proposed swarm-intelligence-based localization algorithm and energy-efficient clustering algorithm for improved wireless coverage of UAV networks.
tags:
  - localization
  - clustering
  - PSO
Year: "2019"
Needs:
Solutions:
Differentiation:
Benefits:
---

[[Localization_and_Clustering_Based_on_Swarm_Intelligence_in_UAV_Networks_for_Emergency_Communications.pdf]]
# Essence
- Answers drone localization through the proposed 3D  swarm intelligence-based localization algorithm   



# Key Findings
* > ([[Localization_and_Clustering_Based_on_Swarm_Intelligence_in_UAV_Networks_for_Emergency_Communications.pdf#page=5&selection=14,0,15,29&color=yellow|p.8962]])
> In this paper, the types of UAV considered can be mini-drones or middle size drones.
 
## Methodology 
> [!important] Simulation Details 
> ![[Pasted image 20261123115137.png]]


>[!note] Assumptions 
>* For localization, the UAVs are equipped with: 
> 	* Intra comms (peer in cluster) - short range wireless comms 
> 	* Intercluster comms (to cluster heads and ground  station) - long-range wireless comms
> * All UAVs are aware of its position, neighbors' positions, and the GS position. 


>[!note] Communication/Network Protocols
>Assessed in **Matlab Network Simulator** 
>1. Intra cluster comms 
>	* IEEE 802.11b 
>	* 2.4 GHz freq band 
>	* 200-250 m range
>	* 11 Mbps of transmission speed
>2. Inter cluster comms
>	* IEEE 802.11n 
>	* 5 GHz
>	* 250-350 m range 
>	* 150-175 Mbps of transmission speed 


>[!note] Network Performance Metrics 
> - Packet Delivery Ratio
> - Average End-to-End Delay 
> - Routing Overhead
> - Energy Consumption



>[!note] Methods 
>**Proposed 6 parts of Algorithm**
>1. Standard PSO Algorithm 
>2. UAV Topology construction and localization with the proposed PSO Algorithm 
>3. Finding the nearest node for cluster formation in 3D 
>4. UAC Clustering 
>5. Cluster head selection 
>6. Multihop routing
> 
>* Bounding box method for localization - estimates the position of the unknown UAV from anchor nodes 
>	* Anchor node - UAV node that knows its position and its neighbors 
>* > ([[Localization_and_Clustering_Based_on_Swarm_Intelligence_in_UAV_Networks_for_Emergency_Communications.pdf#page=5&annotation=1305R|Localization_and_Clustering_Based_on_Swarm_Intelligence_in_UAV_Networks_for_Emergency_Communications, p.8962]])
> n the PSO algorithm, a particle works as an agent in a decentralized system
> 



