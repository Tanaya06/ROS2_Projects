# Node
- Each ROS node is responsible for a single modular purpose. E.g controlling the wheel motors or publishing the sensor data from a laser range-finder.
- Nodes can send & receive data from other nodes via - topics, services, actions or parameters.
## Node related commands
```bash
ros2 node -h # Help

# Run executable
ros2 run <package_name> <executable_name> # E.g ros2 run turtlesim turtlesim_node

# List current running node
ros2 node list

# Remapping allows you to reassign default node properties, like node name, topic names, service names, etc., to custom values.
ros2 run turtlesim turtlesim_node --ros-args --remap __node:=my_turtle

ros2 node info <node_name> # Get node info
```

# Topics
- Topics are a vital element of the ROS graph that act as a bus for nodes to exchange messages.
- Based on Publisher-and-subscriber model
- Node (Publisher) ------(Topic sends message)--------> Node (Subscriber)
- A node may publish data to any number of topics and simultaneously have subscriptions to any number of topics.
- Topics can communicate between one-to-one, one-to-many, many-to-one & many-to-many Nodes.
## Topics related commands
```bash
rqt_graph # Visualizes topics and nodes

ros2 topic list # List running topics

ros2 topic echo <topic_name> # Outputs the topic (message is printed on screen in real time)

ros2 topic info <topic_name> # Get topic info

# Interface: Publishers and subscribers must send and receive the same **type** of message to communicate.
ros2 interface show <msg type>

# ros2 topic pub - you can publish data onto a topic directly from the command line using:
ros2 topic pub <topic_name> <msg_type> '<args>'
```

# Service
- Node (server) ------ (Service) ------> Node (client)
- Another method of communication between nodes
- Based on call-and-response model
- Services only provide data when specifically called by client.
- 
