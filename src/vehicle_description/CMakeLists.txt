cmake_minimum_required(VERSION 2.8.3)
project(vehicle_description)
add_compile_options(-std=c++11)
find_package(catkin REQUIRED)

catkin_package()

install(DIRECTORY launch urdf meshes rviz
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
        PATTERN *.tar.gz EXCLUDE
)
