## Installation

To install **MARUS2 Sensors gRPC** and its required core dependencies, add them directly to your Unity project's **`Packages/manifest.json`** file under the `"dependencies"` block:

```json
{
  "dependencies": {
    "com.labust.marus2.core": "https://github.com/MARUSimulator/marus2-core.git",
    "com.labust.marus2.sensors": "https://github.com/MARUSimulator/marus-sensors.git",
    "com.labust.marus2.sensors-grpc": "https://github.com/MARUSimulator/marus-sensors-grpc.git"
  }
}
```


# Sensor usage
To integrate a gRPC connection inside a Unity scene it is neccessary to attach add a component with format: *gRPC.cs. Sensor data can be acquired through any gRPC server by connecting to a topic listed in the "Address" property of the sensor node.


### ROS

ROS communications are enabled by RosConnection class providing a connection to ROS server. 
To setup ROS backend follow instructions at : https://github.com/MARUSimulator/marus-example/wiki/2.-Installation
and run 

    ros2 launch grpc_ros_adapter ros2_server_launch.py

## Ais
Currently AIS sensor does not provide a ROS connection.

## GPS/GNSS

ROS Topic type: sensor_msgs/msg/NavSatFix 

## IMU

ROS Topic type: sensor_msgs/msg/Imu

## Lidar

ROS Topic type: sensor_msgs/msg/PointCloud2

## Camera

ROS Topic type: sensor_msgs/msg/Image

## Depth sensor


ROS Topic type: geometry_msgs/msg/PoseWithCovarianceStamped


## DVL sensor


ROS Topic type: geometry_msgs/msg/TwistWithCovarianceStamped


## Sonar


ROS topic type: sensor_msgs/msg/Image

## Pose sensor


ROS Topic type: geometry_msgs/msg/PoseWithCovarianceStamped


