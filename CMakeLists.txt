cmake_minimum_required(VERSION 2.8.3)
project(catkin_virtualenv_editable_error)

find_package(catkin REQUIRED COMPONENTS catkin_virtualenv)

catkin_package()
catkin_generate_virtualenv()

include_directories()

install(FILES requirements.txt
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
