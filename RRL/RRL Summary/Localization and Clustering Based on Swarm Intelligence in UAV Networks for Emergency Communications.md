
[[Localization_and_Clustering_Based_on_Swarm_Intelligence_in_UAV_Networks_for_Emergency_Communications.pdf]]
# Essence
- Answers drone localization through the proposed 3D  swarm intelligence-based localization algorithm   



# Key Findings
* Mini-sized and middle-sized drones used 
## Methodology 

>[!todo] Assumptions 
>* For localization, the UAVs are equipped with: 
> 	* Intra comms (peer in cluster) - short range wireless comms 
> 	* Intercluster comms (to cluster heads and ground  station) - long-range wireless comms
> * All UAVs are aware of its position, neighbors' positions, and the GS position. 


>[!todo] Communication/Network Protocols
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


>[!todo] Network Performance Metrics 
> - Packet Delivery Ratio
> - Average End-to-End Delay 
> - Routing Overhead
> - Energy Consumption



>[!todo] Methods 
>* Bounding box method for localization - estimates the position of the unknown UAV from anchor nodes 
>	* Anchor node - UAV node that knows its position and its neighbors 


