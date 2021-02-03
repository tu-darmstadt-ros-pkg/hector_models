^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package hector_xacro_tools
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.5.2 (2021-02-03)
------------------
* Updated package format version, maintainer and CMakeLists.txt to conform to CMP0048.
* Contributors: Stefan Fabian

0.5.1 (2020-12-17)
------------------
* Added velociy transmission
* position interface macro
* Switched to www.ros.org for consistency with ros wiki tutorial and publicly available URDFs.
* Merge pull request `#6 <https://github.com/tu-darmstadt-ros-pkg/hector_models/issues/6>`_ from mipo57/patch-1
  Fix inconsistent namespace warning
* Fix inconsistent namespace warning
  inconsistent namespace redefinitions for xmlns:xacro:
  old: http://www.ros.org/wiki/xacro
  new: http://ros.org/wiki/xacro
  Most of files define url with perciding www. Lack of it results in warning
* Contributors: Martin Oehler, Michał Pogoda, Stefan Fabian

0.5.0 (2018-06-29)
------------------
* Merge branch 'update_transmissions' into kinetic-devel
  Fix xmlns for all xacro files
* Update to transmissions, prepending "hardware_interface/"
* fixed warning
* Add macro for default setting joint properties
* Contributors: Alexander Stumpf, Stefan Kohlbrecher

0.4.2 (2016-06-24)
------------------
* Add joint macros (contains transmission macro for the moment)
* Contributors: Stefan Kohlbrecher

0.4.1 (2015-11-08)
------------------
* hector_xacro_tools: fixed invalid brackets in inertial_sphere* xacro macros
* Cleaned up root element xmlns arguments according to http://gazebosim.org/tutorials?tut=ros_urdf#HeaderofaURDFFile
* Added missing xacro namespace prefix to XML tags
* Contributors: Johannes Meyer

0.4.0 (2015-11-07)
------------------
* Remove origin tag as already set via insert block
* Add additional macros
* Contributors: kohlbrecher

0.3.2 (2014-09-01)
------------------

0.3.1 (2014-03-30)
------------------

0.3.0 (2013-09-02)
------------------
* catkinized stack hector_models
