^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package hector_components_description
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.5.2 (2021-02-03)
------------------
* Updated package format version, maintainer and CMakeLists.txt to conform to CMP0048.
* Contributors: Stefan Fabian

0.5.1 (2020-12-17)
------------------
* added an option to use a gpu accelerated lidar simulation
* Added tracker to vision box
* reduced collision size factor
* added collisoin geometry for table pushing person
* introduced table_link
* updated position on tbale & collision size
* used textured table
* added visionbox on table
* added standalone visionbox urdf
* added a consistent name scheme and xacro name usage
* fixed the inconsistend naming of the xm430 sensor head
* added missing include
* changed file permissions
* unified the GPU and non-GPU VLP16 xacro macro
* added meshes for the XM430 based sensor head
* cleanup
* updated the URDF of the XM430 based sensor head
* updated the URDF of the autonomy box and the VLP16
* Added more missing run dependencies.
* Added missing exec dependency.
* Switched to www.ros.org for consistency with ros wiki tutorial and publicly available URDFs.
* Merge branch 'kinetic-devel' of https://github.com/tu-darmstadt-ros-pkg/hector_models into melodic-devel
* moved t265
* Merge branch 'kinetic-devel' into realsense_t265
* added collision geom to lidar for manipulation
* added raycast geom
* added sensor head collision geometry
* added an URDF for the new XM430 based sensor head
* fixed lidar position
  realsense origin is now in mounting hole
* corrected sizes of autonomy box
* added front/back realsenses to autonomy box
* corrected sizes of autonomy box
* added front/back realsenses to autonomy box
* removed containment filter box for jasmine arm from autonomy box macro
* fixed insta360 and lidar mounting height
* moved autonomy box properties outside of macro scope again
* added parameter to add chilitags in autonomy box macro
* updated realsense t265 macro in autonomy box
* added realsense t265 tracking camera to autonomy box
* Revert "Revert "switched back to new dynamixel controller (which reports positions with an offset of pi)""
  This reverts commit c4d721c81aefe859335de7edfc01bae9bb119c27.
* Revert "switched back to new dynamixel controller (which reports positions with an offset of pi)"
  This reverts commit a9de57af00b22a533b5f1e452efc315a02ba4ca0.
* switched back to new dynamixel controller (which reports positions with an offset of pi)
* Tune mass properties of light links
* Reduce mass of headlight elements
* Modify headlight defaults
* Remove obsolete, commented out code
* Fix autonomy box material color
* Add missing chilitag include (should be removed completely in the future)
  Add imu_link as a param with default
* Fix headlight geom properly. Uses SDF, not URDF syntax
* Fix wrong box geom tag
* Update headlight to remove visuals via plugins available in subt
* Add headlight macro adapted from subt x1 model
* insta 3 exstrinsic calibration
* fixed chilitag position
* rotate the spinning lidar 180° to be compatible to the legacy dynamixel driver
* updated chilitag
* Revert "add sensor head pitch offset"
  This reverts commit 2d99e688ef22209f663ede4f6cfb81a7fc9529b3.
* add sensor head pitch offset
* Increase raycast geometry
* Update kalibr target
  Fix theta mid link to use name param
* moved chilitag
* added thickness of tags
* significatly increased collision model size of insta360
* added collision for insta360 cable
* Add kalibr calibration target
* fixed chilitag rotation
* added chilitag to autonomy box
* adjusted autonomy box sizes
* added collision model to camera360 macro
  added collision model to camera360 mount on autonomy box
* rotated lidar
* added autonomy box macro
* removed unused parts
* Add missing xacro include
* Contributors: Hectorvision, Marius Schnaubelt, Martin Oehler, Stefan Fabian, Stefan Kohlbrecher, Stefan Kohlbrecher (Tracker)

0.5.0 (2018-06-29)
------------------
* Update raycast self filter config for head
* Increase realsense self filter collision size
* Add cylinder geoms for raycast self filtering
* Add macro for being able to set realsense params in more detail
* Update vlp16 mount macro
* Merge branch 'update_transmissions' into kinetic-devel
  Fix xmlns for all xacro files
* Update to transmissions, prepending "hardware_interface/"
* Make tracker sensor head macro independent of vision box properties
* Add plugin for using spinning sensors with gazebo
* Add additional macros of components
* Fix xacro tag
* Merge commit '57d7a25756af77265cfd73298fa5d32' into indigo-devel
* added makro that allows you to define a calibration transformation
* Contributors: Martin Oehler, Stefan Kohlbrecher

0.4.2 (2016-06-24)
------------------
* fixed for checkerboard
* Add checkerboard with associated macro.
* Added calibration and fixed an origin bug at the spinnning joint of the lidar
* Added realistic inertias and masses. Moved RGB-D Cam according to reality
* Contributors: Marius Schnaubelt, Martin Oehler, Stefan Kohlbrecher

0.4.1 (2015-11-08)
------------------
* hector_components_description/hector_sensors_description: added xacro namespace prefix to macro calls
* Cleaned up root element xmlns arguments according to http://gazebosim.org/tutorials?tut=ros_urdf#HeaderofaURDFFile
* Added missing xacro namespace prefix to XML tags
* Contributors: Johannes Meyer

0.4.0 (2015-11-07)
------------------
* Renamed LIDAR and RGBD cam for thor compatibility
* Remove gazebo tags for links without visuals
* First version of the new head, the hector multisensor head
* Add addons xacro files
* Update how spinning hokuyo is set up
* Update spinning lidar mount properties
* Fix stupid mixup of min and max lidar angle
* Reduce spinning lidar mount mass
* Fix parent not used correctly in spinning lidar mount
* Update rotating hokuyo transform
* Refactor spinning lidar mount
* Update LIDAR mount with reasonable inertia
* URDF hardware interface changes for new gazebo ros control style (#185)
* Add second spinning hokuyo variant
* Fix origin block not getting used correctly
* Add gazebo_ros_control required tags to spinning lidar macros
* Formatting
* Add spinning lidar mount and hokuyo example
* Contributors: Marius Schnaubelt, Stefan Kohlbrecher

0.3.2 (2014-09-01)
------------------
* increased maximum torque for camera servos in vision_box_common.gazebo.xacro
* adapted urdf for asus xtion and added camera variables
* Add simple ps eye geometry
* Contributors: Johannes Meyer, Stefan Kohlbrecher

0.3.1 (2014-03-30)
------------------
* Re-parent LIDAR and camera mount to top_box_link
* Add xacro macros for setting dimensions
* Remove obsolete files
* Add UTM-30LX macro to vision box xacro
* Add hector ugv vision box to hector_components_description package for better reusability
* Contributors: Stefan Kohlbrecher
