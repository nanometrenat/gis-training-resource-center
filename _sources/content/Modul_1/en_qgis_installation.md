# Installation

QGIS is an open source geoinformation system software for viewing, editing, capturing and analyzing spatial data and and to create printable maps. QGIS has been since 2002 and is a project of volunteers. 
You can install QGIS for Windows, Mac and Linux computers. 

## Windows
For the installation under Windows we use the OSGeo4W network installer. OSGeo4W is a project that offers Open Geo related software for Windows easy to install. Visit the project page [https://trac.osgeo.org/osgeo4w/](https://trac.osgeo.org/osgeo4w/) and click there on the link `Download the ​OSGeo4W network installer`. 

* Make sure to select _Advanced Install_ / _Fortgeschrittene Installation_ during the installation process. Only then can you accurately select the software relevant to this course:
   - QGIS Desktop
   - GRASS GIS
   - SAGA
  
Video tutorial: https://www.youtube.com/watch?v=pja_EX0tVZA

The selected software is then downloaded via the Internet and installed on-the-fly.

## Mac

__**From version 3.30 SAGA must be integrated via plugin**__

At https://qgis.org/en/site/forusers/download.html select `Download for macOS`, then use the link _Download QGIS_. 

In QGIS then install the plugin _Processing Saga NextGen Provider_. 

More about how to install and activate plugins in QGIS can be found here:
[qgis-Interface#erweiterungen-plugins-installieren](https://courses.gistools.geog.uni-heidelberg.de/giscience/gis-einfuehrung/-/wikis/qgis-Interface#erweiterungen-plugins-installieren)

## Linux

__**From version 3.30 SAGA must be integrated via plugin**__

For installation on Linux systems with apt you can install QGIS:

```
sudo apt install qgis qgis-plugin-grass
```

In the conventional apt package sources, an older version of QGIS will probably be installed. If you use the package source [Ubuntugis](https://launchpad.net/~ubuntugis/+archive/ubuntu/ppa), please note the following installation hints at https://qgis.org/en/site/forusers/alldownloads.html#repositories

If you want to install a QGIS version >3.30 you have to install the plugin _Processing Saga NextGen Provider_.  

More about how to install and activate plugins in QGIS can be found here:
[qgis-Interface#erweiterungen-plugins-installieren](https://courses.gistools.geog.uni-heidelberg.de/giscience/gis-einfuehrung/-/wikis/qgis-Interface#erweiterungen-plugins-installieren)
 
