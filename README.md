# install-opencv

## Updating Linux
`sudo apt-get update`

`sudo apt-get upgrade`

## Install Dependecies
`sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev`

`sudo apt-get install python3-dev python3-numpy libtbb2 libtbb-dev`

`sudo apt-get install libjpeg-dev`

 `sudo apt-get install libpng-dev`
 
 `sudo apt-get install libtiff5-dev`
 
 `sudo apt-get install jasper`
 
 `sudo apt-get install libdc1394-22-dev`
 
 `sudo apt-get install libeigen3-dev`
 
 `sudo apt-get install libtheora-dev`
 
 `sudo apt-get install libvorbis-dev`
 
 `sudo apt-get install libxvidcore-dev`
 
 `sudo apt-get install libx264-dev`
 
 `sudo apt-get install sphinx-common`
 
 `sudo apt-get install libtbb-dev`
 
 `sudo apt-get install yasm`
 
 `sudo apt-get install libfaac-dev`
 
 `sudo apt-get install libopencore-amrnb-dev`
 
 `sudo apt-get install libopencore-amrwb-dev`
 
 `sudo apt-get install libopenexr-dev`
 
 `sudo apt-get install libgstreamer-plugins-base1.0-dev`
 
 `sudo apt-get install libavutil-dev`
 
 `sudo apt-get install libavfilter-dev`
 
 `sudo apt-get install libavresample-dev`
 
 ## Set Installation Path and Get Opencv
 `sudo -s`
 
 `cd /opt`
 
 `git clone https://github.com/opencv/opencv.git`
 
 `cd opencv`
 
 `git checkout 3.4.0`
 
 `cd ..`
 
 `git clone https://github.com/Itseez/opencv_contrib.git`
 
 `cd opencv_contrib`
 
 `git checkout 3.4.0`
 
 `cd ..`
 
 ## Install Opencv and Opencv Contrib
 `cd opencv`
 
 `mkdir release`
 
 `cd release`
 
 `cmake -D BUILD_TIFF=ON -D WITH_CUDA=OFF -D ENABLE_AVX=OFF -D WITH_OPENGL=OFF -D WITH_OPENCL=OFF -D WITH_IPP=OFF -D WITH_TBB=ON -D BUILD_TBB=ON -D WITH_EIGEN=OFF -D WITH_V4L=OFF -D WITH_VTK=OFF -D BUILD_TESTS=OFF -D BUILD_PERF_TESTS=OFF -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local -D OPENCV_EXTRA_MODULES_PATH=/opt/opencv_contrib/modules /opt/opencv/`
 
 `make -j4`
 
 `make install`
 
 `ldconfig`
 
 `exit`
 
 ## Test Installation
 
 `pkg-config --modversion opencv` 
 
 
 
 
