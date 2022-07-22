# dmq (Direct Memory Queue)
Building Cloud Native Dataplane :  zero-copy packet interface between VPP, DPDK and cloud native services 

This project aims at building a zero-copy packet framework for multiple dataplane technologies (e.g.DPDK and VPP) and value added services (DPI, IPS) and cloud native applications. The traditional dataplanes (VPP or DPDK based) are large monolith and hard to scale out. It's challenging to pass packets between two dataplanes without memory copy. The value added services (IPS, DPI, Proxy, NAT-ALG etc) are often provided by 3rd party and is hard to integrate in the dataplane. Inline packet processing of these application in the dataplane often negatively affects packet forwarding performance.  

This project inspired by CNDP (https://community.intel.com/t5/Blogs/Tech-Innovation/Edge-5G/Cloud-Native-Data-Plane-CNDP-Enabling-a-cloud-based-framework/post/1381808) to bridge the gap between traditional dataplanes and the requirements of todays cloud native world. 

It also has the ambitious goal of interoperating dataplanes with other Linux Kernel based zero-copy packet processing techologies such as AF_XDP (https://docs.kernel.org/networking/af_xdp.html)             
