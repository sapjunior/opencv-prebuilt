# OpenCV 3.4.3 with Contrib Modules Prebuilt Binary (AVX2 Optimization)

## Prerequisites 
- AVX2 CPU
- Ubuntu 18.04 (Default Python 3.6)

## Packages
sudo apt install python-dev python3-dev python-numpy python3-numpy ccache zlibc libjpeg-dev libtiff-dev libwebp-dev libpng-dev libopenexr-dev libgtk2.0-dev libgtk-3-dev libdc1394-22-dev ffmpeg libavcodec-dev libavformat-dev libavutil-dev libswscale-dev libavresample-dev libatlas-base-dev libatlas-cpp-0.6-dev libblas-dev liblapack-dev liblapacke-dev openjdk-8-jdk ant git libopenexr-dev libeigen3-dev libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev libv4l-dev libgflags-dev libgoogle-glog-dev hdf5-tools libhdf5-dev libtesseract-dev libleptonica-dev libceres-dev 

## Install
sudo dpkg -i <filename>.deb

## Remove
sudo apt remove opencv-contrib

## CMake Options
-DENABLE_FAST_MATH:BOOL="1" -DOPENCV_EXTRA_MODULES_PATH:PATH="/home/thananop/Workspace/opencv/opencv_contrib-3.4.3/modules" -DCPU_BASELINE:STRING="AVX2" -DOPENCV_ENABLE_NONFREE:BOOL="1" -DENABLE_CXX11:BOOL="1" 

## cv2.getBuiltInformation()
General configuration for OpenCV 3.4.3 =====================================
  Version control:               unknown

  Extra modules:
    Location (extra):            /home/thananop/Workspace/opencv/opencv_contrib-3.4.3/modules
    Version control (extra):     unknown

  Platform:
    Timestamp:                   2018-10-08T13:47:13Z
    Host:                        Linux 4.15.0-36-generic x86_64
    CMake:                       3.10.2
    CMake generator:             Unix Makefiles
    CMake build tool:            /usr/bin/make
    Configuration:               Release

  CPU/HW features:
    Baseline:                    SSE SSE2 SSE3 SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2
      requested:                 AVX2
    Dispatched code generation:  AVX512_SKX
      requested:                 SSE4_1 SSE4_2 AVX FP16 AVX2 AVX512_SKX
      AVX512_SKX (1 files):      + AVX_512F AVX512_SKX

  C/C++:
    Built as dynamic libs?:      YES
    C++11:                       YES
    C++ Compiler:                /usr/bin/c++  (ver 7.3.0)
    C++ flags (Release):         -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wsuggest-override -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffast-math -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -mssse3 -msse4.1 -mpopcnt -msse4.2 -mf16c -mfma -mavx -mavx2 -fvisibility=hidden -fvisibility-inlines-hidden -O3 -DNDEBUG  -DNDEBUG
    C++ flags (Debug):           -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wsuggest-override -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffast-math -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -mssse3 -msse4.1 -mpopcnt -msse4.2 -mf16c -mfma -mavx -mavx2 -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
    C Compiler:                  /usr/bin/cc
    C flags (Release):           -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Winit-self -Wno-narrowing -Wno-comment -Wimplicit-fallthrough=3 -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffast-math -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -mssse3 -msse4.1 -mpopcnt -msse4.2 -mf16c -mfma -mavx -mavx2 -fvisibility=hidden -O3 -DNDEBUG  -DNDEBUG
    C flags (Debug):             -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Winit-self -Wno-narrowing -Wno-comment -Wimplicit-fallthrough=3 -fdiagnostics-show-option -Wno-long-long -pthread -fomit-frame-pointer -ffast-math -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -mssse3 -msse4.1 -mpopcnt -msse4.2 -mf16c -mfma -mavx -mavx2 -fvisibility=hidden -g  -O0 -DDEBUG -D_DEBUG
    Linker flags (Release):      
    Linker flags (Debug):        
    ccache:                      YES
    Precompiled headers:         NO
    Extra dependencies:          dl m pthread rt
    3rdparty dependencies:

  OpenCV modules:
    To be built:                 aruco bgsegm bioinspired calib3d ccalib core datasets dnn dnn_objdetect dpm face features2d flann freetype fuzzy hdf hfs highgui img_hash imgcodecs imgproc java java_bindings_generator line_descriptor ml objdetect optflow phase_unwrapping photo plot python2 python3 python_bindings_generator reg rgbd saliency sfm shape stereo stitching structured_light superres surface_matching text tracking ts video videoio videostab xfeatures2d ximgproc xobjdetect xphoto
    Disabled:                    js world
    Disabled by dependency:      -
    Unavailable:                 cnn_3dobj cudaarithm cudabgsegm cudacodec cudafeatures2d cudafilters cudaimgproc cudalegacy cudaobjdetect cudaoptflow cudastereo cudawarping cudev cvv matlab ovis viz
    Applications:                tests perf_tests apps
    Documentation:               NO
    Non-free algorithms:         YES

  GUI: 
    GTK+:                        YES (ver 3.22.30)
      GThread :                  YES (ver 2.56.2)
      GtkGlExt:                  NO
    VTK support:                 NO

  Media I/O: 
    ZLib:                        /usr/lib/x86_64-linux-gnu/libz.so (ver 1.2.11)
    JPEG:                        /usr/lib/x86_64-linux-gnu/libjpeg.so (ver 80)
    WEBP:                        /usr/lib/x86_64-linux-gnu/libwebp.so (ver encoder: 0x020e)
    PNG:                         /usr/lib/x86_64-linux-gnu/libpng.so (ver 1.6.34)
    TIFF:                        /usr/lib/x86_64-linux-gnu/libtiff.so (ver 42 / 4.0.9)
    JPEG 2000:                   build (ver 1.900.1)
    OpenEXR:                     /usr/lib/x86_64-linux-gnu/libImath.so /usr/lib/x86_64-linux-gnu/libIlmImf.so /usr/lib/x86_64-linux-gnu/libIex.so /usr/lib/x86_64-linux-gnu/libHalf.so /usr/lib/x86_64-linux-gnu/libIlmThread.so (ver 2.2.0)
    HDR:                         YES
    SUNRASTER:                   YES
    PXM:                         YES

  Video I/O:
    DC1394:                      YES (ver 2.2.5)
    FFMPEG:                      YES
      avcodec:                   YES (ver 57.107.100)
      avformat:                  YES (ver 57.83.100)
      avutil:                    YES (ver 55.78.100)
      swscale:                   YES (ver 4.8.100)
      avresample:                YES (ver 3.7.0)
    GStreamer:                   
      base:                      YES (ver 1.14.1)
      video:                     YES (ver 1.14.1)
      app:                       YES (ver 1.14.1)
      riff:                      YES (ver 1.14.1)
      pbutils:                   YES (ver 1.14.1)
    libv4l/libv4l2:              NO
    v4l/v4l2:                    linux/videodev2.h

  Parallel framework:            pthreads

  Trace:                         YES (with Intel ITT)

  Other third-party libraries:
    Intel IPP:                   2017.0.3 [2017.0.3]
           at:                   /home/thananop/Workspace/opencv/build-3.4.3/3rdparty/ippicv/ippicv_lnx
    Intel IPP IW:                sources (2017.0.3)
              at:                /home/thananop/Workspace/opencv/build-3.4.3/3rdparty/ippicv/ippiw_lnx
    Lapack:                      YES (/usr/lib/x86_64-linux-gnu/liblapack.so /usr/lib/x86_64-linux-gnu/libcblas.so /usr/lib/x86_64-linux-gnu/libatlas.so)
    Eigen:                       YES (ver 3.3.4)
    Custom HAL:                  NO
    Protobuf:                    build (3.5.1)

  OpenCL:                        YES (no extra features)
    Include path:                /home/thananop/Workspace/opencv/opencv-3.4.3/3rdparty/include/opencl/1.2
    Link libraries:              Dynamic load

  Python 2:
    Interpreter:                 /usr/bin/python2.7 (ver 2.7.15)
    Libraries:                   /usr/lib/x86_64-linux-gnu/libpython2.7.so (ver 2.7.15rc1)
    numpy:                       /usr/lib/python2.7/dist-packages/numpy/core/include (ver 1.13.3)
    packages path:               lib/python2.7/dist-packages

  Python 3:
    Interpreter:                 /usr/bin/python3 (ver 3.6.6)
    Libraries:                   /usr/lib/x86_64-linux-gnu/libpython3.6m.so (ver 3.6.6)
    numpy:                       /usr/lib/python3/dist-packages/numpy/core/include (ver 1.13.3)
    packages path:               lib/python3.6/dist-packages

  Python (for build):            /usr/bin/python2.7

  Java:                          
    ant:                         /usr/bin/ant (ver 1.10.3)
    JNI:                         /usr/lib/jvm/java-8-openjdk-amd64/include /usr/lib/jvm/java-8-openjdk-amd64/include/linux /usr/lib/jvm/java-8-openjdk-amd64/include
    Java wrappers:               YES
    Java tests:                  YES

  Matlab:                        NO

  Install to:                    /usr/local
-----------------------------------------------------------------

