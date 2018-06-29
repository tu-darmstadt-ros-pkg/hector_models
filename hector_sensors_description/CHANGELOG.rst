^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package hector_sensors_description
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
