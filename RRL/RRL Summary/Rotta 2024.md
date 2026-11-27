---
Title: "[[B.A.T.M.A.N._Mesh_Networking_on_ESP32s_802.11.pdf]]"
Year: "2024"
Author/s: Rotta, Schulz, Naumann, Chatharajupalli, Nolte, Werner
Publication: IEEE Conference on Local Computer Networks
Category: "[[UAV Comm Protocol]]"
Bibtex: "@INPROCEEDINGS{10639698,\r

  \  author={Rotta, Randolf and Schulz, Julius and Naumann, Billy and Chatharajupalli, Navya Sneha and Nolte, Jörg and Werner, Matthias},\r

  \  booktitle={2024 IEEE 49th Conference on Local Computer Networks (LCN)}, \r

  \  title={B.A.T.M.A.N. Mesh Networking on ESP32’s 802.11}, \r

  \  year={2024},\r

  \  volume={},\r

  \  number={},\r

  \  pages={1-7},\r

  \  keywords={Wireless communication;Performance evaluation;Mesh networks;Wireless sensor networks;TCPIP;Throughput;Routing protocols;Ad hoc networks;Wireless mesh networks},\r

  \  doi={10.1109/LCN60385.2024.10639698}}"
---
> ([[B.A.T.M.A.N._Mesh_Networking_on_ESP32s_802.11.pdf#page=1&selection=55,50,64,60&color=yellow|B.A.T.M.A.N._Mesh_Networking_on_ESP32s_802.11, p.1]])
> The Better Approach To Mobile Ad-Hoc Networks (B.A.T.M.A.N.) is a popular mesh protocol [1], [2], which was initially developed by the Freifunk community to<mark style="background:#fff88f"> build free and open mesh networks.</mark> It proactively maintains the <mark style="background:#fff88f">best route</mark> between each pair of nodes <mark style="background:#fff88f">based on the estimated end-to-end throughput.</mark>

**Differentiation**
**Contrasts the use of ESP NOW and ESP MESH WIFI **
> ([[B.A.T.M.A.N._Mesh_Networking_on_ESP32s_802.11.pdf#page=1&selection=169,53,172,21&color=yellow|B.A.T.M.A.N._Mesh_Networking_on_ESP32s_802.11, p.1]])
> Unlike Espressif’s proprietary Wi-Fi mesh, <mark style="background:#fff88f">our routing is not limited to a tree topology </mark>and, hence, can connect any nodes on the best direct path.

> ([[B.A.T.M.A.N._Mesh_Networking_on_ESP32s_802.11.pdf#page=1&annotation=174R|B.A.T.M.A.N._Mesh_Networking_on_ESP32s_802.11, p.1]])
>  We also utilize full 1500 byte frames

# Methodology
* No protocol seem to exist for BATMAN so it  based on Linux kernel's implementation details a
*  Very technical implementation in the low-level driver of WiFi at Layer 2 




# Supplemented/Cited Works 

[[A_Modular_Communication_Architecture_for_Adaptive_UAV_Swarms.pdf]] 
- [[A_Modular_Communication_Architecture_for_Adaptive_UAV_Swarms.pdf#page=3&selection=291,3,291,43&color=yellow|Implications for the Swarm Communication]] -**needs** for the literature 
