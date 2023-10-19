
## Services :

Services are another way that nodes can communicate with each other. Services allow nodes to send a request and receive a response.



### Rosservice : 
rosservice can easily attach to ROS's client/service framework with services. rosservice has many commands that can be used on services, as shown below:

```
rosservice list         print information about active services
rosservice call         call the service with the provided args
rosservice type         print service type
rosservice find         find services by service type
rosservice uri          print service ROSRPC uri
```
### ROS RQT :

rqt_console attaches to ROS's logging framework to display output from nodes. rqt_logger_level allows us to change the verbosity level (DEBUG, WARN, INFO, and ERROR) of nodes as they run.

```
rosrun rqt_console rqt_console
rosrun rqt_logger_level rqt_logger_level
```
service vs topics:
Topics are used to send/recieve continuous stream of data. 
services are used generally for singular event based data calls. 
