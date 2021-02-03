^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package hector_sensors_description
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.5.2 (2021-02-03)
------------------
* Updated package format version, maintainer and CMakeLists.txt to conform to CMP0048.
* Contributors: Stefan Fabian

0.5.1 (2020-12-17)
------------------
* Merge branch 'kinetic-devel' of https://github.com/tu-darmstadt-ros-pkg/hector_models into melodic-devel
* Added missing xacro include to vlp16 macro
* Added missing xacro include to vlp16 macro
* Matching vive tracker color to gazebo color
* Replaced vive tracker collision with bounding box and added color
* Changed tracker simulation topic and color
* added 3d model
* added gazebo params
* added new urdf
* Merge pull request `#8 <https://github.com/tu-darmstadt-ros-pkg/hector_models/issues/8>`_ from TheMangalex/kinetic-devel
  Vive Tracker Urdf
* added 3d model
* added gazebo params
* added new urdf
* Set gazebo cam distortion params too
* Added parametrized camera macro
* zoom cam mesh
* flir housing mesh
* tis zoom cam
* unified the GPU and non-GPU VLP16 xacro macro
* updated the URDF of the autonomy box and the VLP16
* cleanup
* added the flir boson 640 thermal cam
* Added more missing run dependencies.
* Fixed dependencies and install rules.
* Switched to www.ros.org for consistency with ros wiki tutorial and publicly available URDFs.
* Merge branch 'kinetic-devel' of https://github.com/tu-darmstadt-ros-pkg/hector_models into melodic-devel
* use a prettier D435 model
* fixed insta360 cam size
* added high res visuals for vlp16
* added macro for realsense with mount
* added a seek thermal macro without geometry
* fixed missing arg tag
* added second tracking frame with the convention of the datasheet
* renamed camera link to camera pose frame to match rs driver names
* Revert "added t265 pose frame". Pose frame is published by driver in tf.
  This reverts commit e11f9f1f9932411b386e5cf1d749a6e92a17d46c.
* added t265 pose frame
* Merge branch 'kinetic-devel' into realsense_t265
* removed collision size prop
* added raycast geom
* added sensor head collision geometry
* added an URDF for the new XM430 based sensor head
* Merge branch 'kinetic-devel' into autonomy_box_cage_realsenses
* added new d435 macro with origin in mounting hole
* Merge branch 'kinetic-devel' into autonomy_box_cage_realsenses
* more refactoring and added option to use realsense d435 mesh
* added static publisher launch for d435 frames
* fixed visual and collision of d435
* d435 macro refactoring
* renamed realsense t265 macros
* added realsense t265 description
* fixed default topic
* Comment out custom lens due to gazebo segfaults on some machines
* Update camera360 to params we could calibrate with kalibr
* Update kalibr target
  Fix theta mid link to use name param
* fixed cam frame orientation
* Make resolution params and set defaults for thermal cam
* fixed default collision radius
* moved chilitag
* added collision for insta360 cable
* added collision model to camera360 macro
  added collision model to camera360 mount on autonomy box
* fix D435 macro
* added parameter for dist between cams to camera360 macro
* Contributors: Alberto Romay, Frederik, Frederik Bark, Marius Schnaubelt, Martin Oehler, Stefan Fabian, Stefan Kohlbrecher

0.5.0 (2018-06-29)
------------------
* added calibration parameter
* added macro for generic 360 cameras
* add the realsense D435
* Add macro for being able to set realsense params in more detail
* Update VLP16 macro to provide normal and advanced versions
* Properly use cameraName tag and topics relative to camera namespace
* Fix ricoh_theta camera name and topic setup
* Add ricoh_theta model usable with gazebo8+
* Merge branch 'kinetic-devel' of https://github.com/tu-darmstadt-ros-pkg/hector_models into kinetic-devel
* Merge branch 'update_transmissions' into kinetic-devel
  Fix xmlns for all xacro files
* Merge pull request `#5 <https://github.com/tu-darmstadt-ros-pkg/hector_models/issues/5>`_ from cschindlbeck/fix_include_in_kinect
  Fix missing include in kinect_camera
* Reduce vlp16 min range
* Fix missing include in kinect
* Optimize simulated vlp16 for performance
* fixed warning
* Add optional macro for setting realsense topics
* Reduce min range for Realsense as we're mostly interested in rgb data for now
* Fix R200 FOV to be in line with real camera
* Switch to using velodyne_simulator
* VLP-16 basics
* changed minimal laser scanner distance
* Fix coloring for simulated depth cameras (RGB vs BGR)
  See https://bitbucket.org/osrf/gazebo/issues/1865/rendering-depthcamera-does-not-output
* Adjust realsense FOV to be in line with real rgb sensor FOV
* Modify realsense r200 macro to also make version without geometry available
* Merge commit '57d7a25756af77265cfd73298fa5d32' into indigo-devel
* Change thermal cam default topic name to image_raw instead of image
* Move cam link to where real realsense driver expects it (rgb cam frame)
* Remove frames as part of model as they are published based on internal intrinsics on real sensor
* Corrected realsense frames and measures
* Image topic corrected
* Changed resolution to match real cam
* Contributors: Alexander Stumpf, Chris Schindlbeck, Christian Rose, Marius Schnaubelt, Martin Oehler, Philipp Schillinger, Stefan Kohlbrecher

0.4.2 (2016-06-24)
------------------
* Update flir a35 camera macro
* Add gazebo material for flir and realsense models
* Add models for flir a35 and realsense r200 cameras
* Formatting of thermaleye_camera macro
* Contributors: Stefan Kohlbrecher

0.4.1 (2015-11-08)
------------------
* hector_components_description/hector_sensors_description: added xacro namespace prefix to macro calls
* Cleaned up root element xmlns arguments according to http://gazebosim.org/tutorials?tut=ros_urdf#HeaderofaURDFFile
* hector_sensors_description: removed deprecated plugin parameters and added noise to the hokuyo_utm30lx_model macro (fix #1)
* Contributors: Johannes Meyer

0.4.0 (2015-11-07)
------------------
* Add zoom camera xacro macro. Only works starting with Gazebo6
* Update asus_camera.urdf.xacro
  Clarify macro use.
* Remove link geometries where not needed
  Add generic_thermal_camera macro
* Update how spinning hokuyo is set up
* Update hokuyo gpu xacro macro
* Properly use camera name
* changed asus description, collision geometry needs to match visual geometry for 3d self filter to work.
* Add generic stereo camera macro
* Use cylinder collision geom as box gives spurious errors in LIDAR scans in some URDFs
* Contributors: Florian Kunz, Stefan Kohlbrecher

0.3.2 (2014-09-01)
------------------
* Updated asus xtion pro live mesh to reflect actual sensor dimensions, add stl version
* Contributors: Stefan Kohlbrecher

0.3.1 (2014-03-30)
------------------
* added hokuyo_utm30lx_model and hokuyo_utm30lx_gpu macros and disabled gpu laser in default hokuyo_utm30lx macro
* use gpu_ray sensor in hydro
* Contributors: Johannes Meyer

0.3.0 (2013-09-02)
------------------
* catkinized stack hector_models
