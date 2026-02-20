cmake_minimum_required(VERSION 3.5)
project(marty1_description)

if(NOT CMAKE_BUILD_TYPE AND NOT CMAKE_CONFIGURATION_TYPES)
  set(CMAKE_BUILD_TYPE Release)
endif()

find_package(ament_cmake_ros REQUIRED)

# Installation...

install(DIRECTORY urdf DESTINATION share/${PROJECT_NAME})

install(DIRECTORY launch DESTINATION share/${PROJECT_NAME})

ament_package()
