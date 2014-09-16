cmake_minimum_required(VERSION 2.8.3)
project(pr2_make_a_map_app)
find_package(catkin REQUIRED COMPONENTS pr2_position_scripts gmapping tf topic_tools map_store)

catkin_package(
    DEPENDS 
    CATKIN_DEPENDS pr2_position_scripts gmapping tf topics_tools_map_store# TODO
    INCLUDE_DIRS # TODO include
    LIBRARIES # TODO
)

install(FILES make_a_map.app make_a_map.interface make_a_map.launch slam_gmapping.xml map.jpg DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
