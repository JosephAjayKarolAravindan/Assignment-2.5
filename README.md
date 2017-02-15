1.	Explain what is a cluster and what is a Hadoop cluster:

A cluster is a group of servers and other resources that act like a single system and enable high availability and, in some cases, load balancing and parallel processing. 
A Hadoop cluster is a special type of computational cluster designed specifically for storing and analyzing huge amounts of unstructured data in a distributed computing environment. 

2.	What is meant by a Rack and explain the rack arrangement in a Hadoop cluster:

A Node is simply a computer. This is typically non-enterprise, commodity hardware for nodes that contain data. Storage of Nodes is called as rack. A rack is a collection of 30 or 40 nodes that are physically stored close together and are all connected to the same network switch. Network bandwidth between any two nodes in rack is greater than bandwidth between two nodes on different racks. A Hadoop Cluster is a collection of racks.
Hadoop Cluster would consists of
•	110 different racks
•	Each rack would have around 40 slave machine
•	At the top of each rack there is a rack switch
•	Each slave machine(rack server in a rack) has cables coming out it from both the ends
•	Cables are connected to rack switch at the top which means that top rack switch will have around 80 ports
•	There are global 8 core switches
•	The rack switch has uplinks connected to core switches and hence connecting all other racks with uniform bandwidth, forming the Cluster
•	In the cluster, few machines to act as Name node and as JobTracker. They are referred as Masters. These masters have different configuration favoring more DRAM and CPU and less local storage.
•	The majority of the machines acts as DataNode and Task Trackers and are referred as Slaves. These slave nodes have lots of local disk storage and moderate amounts of CPU and DRAM

