
Basic Descriptions:

  * **Nodes**: A node is an executable that uses ROS to communicate with other nodes.
  * **Messages**: ROS data type used when subscribing or publishing to a topic.
  * **Topics**: Nodes can publish messages to a topic as well as subscribe to a topic to receive messages.
  * **Master**: Name service for ROS (i.e. helps nodes find each other)
  * **rosout**: ROS equivalent of stdout/stderr
  * **roscore**: Master + rosout + parameter server (parameter server will be introduced later)

## Rqt Graph
Run rqt_graph command creates a dynamic graph of what's going on in the system. Run to see a map of the publishers and subscriber
```
rosrun rqt_graph rqt_graph
```


## Rostopic
* *rostopic -h* is for help
* *rostopic echo topicname* :   shows the data published on a topic.
* *rostopic list*: returns a list of all topics currently subscribed to and published.
  * *-h*: help
  * *-v*: verbose with all details
  * rostopic type [topic] to show data type of topic
  * rosmsg show geometry_msgs/Twist to see details of the message type
  * rostopic pub [topic] [msg_type] [args]
  * rostopic hz reports the rate at which data is published.
* rosrun rqt_plot rqt_plot : displays a scrolling time plot of the data published on topics. 
