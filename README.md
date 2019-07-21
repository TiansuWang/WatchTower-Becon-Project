# WatchTower-Becon-Project
> This project is the outcome of Tiansu Wang during the internship at WatchTower Robotics

This project create a wireless sensor network to locate robot in plastic/cement pipes.


## How it works
![basic concept](/system_diagram/operational_chart/basic_concept.png)

+ The leak detection robot which run along the pipeline can generate radio signal.
+ We put sensor nodes(node0, node1 and node2 in diagram) along the pipeline. 
+ When the robot approaches one sensor node, the node can capture the RF signal so that we know at this time robot is running under this sensor node. Then the sensor node register this time stamp.
+ The sensor node will send the data package (including GPS location and passing time stamp) to the control center which can be a laptop or a portal device.

## repository catalog
> a_node_GUI_2  _UI designed for laptop as a control center._
> beacon_node_folder _Arduino code installed in the sensor node_
> configure_node_folder _Arduino code installed in transceiver which connected to laptop via serial port. Such that the laptop(control center) is able to transmit command and receive data._
> relay_node_folder _Arduino code in relay node, which placed between two sensor nodes help relaying signal. Only needed when two adjacent sensor nodes is too far. ‌_
> system_diagram _Program flow charts, operation instruction diagram_



