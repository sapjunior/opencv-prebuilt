#OpenCV 3.4.3 with Contrib Modules Prebuilt Binary (AVX2 Optimization)

##Prerequisites 
- AVX2 CPU
- Ubuntu 18.04 (Default Python 3.6)

##Packages
sudo apt install python-dev python3-dev python-numpy python3-numpy ccache zlibc libjpeg-dev libtiff-dev libwebp-dev libpng-dev libopenexr-dev libgtk2.0-dev libgtk-3-dev libdc1394-22-dev ffmpeg libavcodec-dev libavformat-dev libavutil-dev libswscale-dev libavresample-dev libatlas-base-dev libatlas-cpp-0.6-dev libblas-dev liblapack-dev liblapacke-dev openjdk-8-jdk ant git libopenexr-dev libeigen3-dev libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev libv4l-dev libgflags-dev libgoogle-glog-dev hdf5-tools libhdf5-dev libtesseract-dev libleptonica-dev libceres-dev 

##Install
sudo dpkg -i <filename>.deb

##Remove
sudo apt remove opencv-contrib

##CMake Options
-DENABLE_FAST_MATH:BOOL="1" -DOPENCV_EXTRA_MODULES_PATH:PATH="/home/thananop/Workspace/opencv/opencv_contrib-3.4.3/modules" -DCPU_BASELINE:STRING="AVX2" -DOPENCV_ENABLE_NONFREE:BOOL="1" -DENABLE_CXX11:BOOL="1" 

