# Datacenter-Network-Simulation-using-ns3 

## Objective
  * Simulate a datacenter network using ns3.
  * Experiment two traffic patterns.
  * Examine the network.
  * Improve the network.

## Topology
<div align=center>
    <img width="759" height="300" src="https://github.com/fox6666/Datacenter-Network-Simulation-using-ns3/blob/master/image/network.png"       "网络拓扑图"/>
</div>

## Description
  * 8 servers: n1\~8; 4 ToR switches: t1\~4; 2 aggregation switches: a1\~2; 1 core switch: c1
  * The network is partitioned into two clusters.
  * The links connecting to c1 are PPP, and the others are Ethernets. The networks’ capacities are shown on the topology graph.
  * All the end-end delays on the networks are 500ns.
  * IP address assignment is shown on the topology.
  * All the switches behave like OSPF routers.
  
## Traffic patterns
 * Pattern 1: inter-cluster traffic
   * Each server communicates using TCP with another server that comes from a different cluster
     * For example, 1-5, 6-2, 3-7, 8-4
 * Pattern 2: many-to-one traffic
   * Select one server as the sink, and all the other servers communicate to it
 * Simulate the two patterns separately, obtain the throughput that the network can achieve, and find out the network bottleneck, and how to improve the network.

