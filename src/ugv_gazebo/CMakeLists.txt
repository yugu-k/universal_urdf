cmake_minimum_required(VERSION 3.8)
project(ugv_gazebo)

find_package(ament_cmake REQUIRED)
find_package(rclcpp REQUIRED)
find_package(gazebo_ros REQUIRED)
find_package(ugv_description REQUIRED)          
find_package(robot_state_publisher REQUIRED)

install(DIRECTORY urdf launch
  DESTINATION share/${PROJECT_NAME}
)

ament_package()
