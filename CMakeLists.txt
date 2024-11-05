cmake_minimum_required(VERSION 3.5)
project(hector_models VERSION 0.5.1)

# Find necessary packages
find_package(ament_cmake REQUIRED)

install(DIRECTORY
  launch
  meshes
  urdf
  gazebo
  DESTINATION share/${PROJECT_NAME}
)

ament_environment_hooks(hooks/${PROJECT_NAME}.dsv.in)
ament_environment_hooks(hooks/${PROJECT_NAME}.sh.in)

# Mark the package as an ament package
ament_package()
