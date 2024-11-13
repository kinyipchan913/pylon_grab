# pylon_grab
Example of build and run OpenCV on Windows using CMake build with CMakeLists.txt
Tested on Ubuntu 20.04
OpenCV 4.2.0
CMake 3.16.3
VS code

## Dependencies
The following applications are used to build Pylon grab example:
- [CMake](https://cmake.org/)  
The following libraries are used by Pylon grab example:
- [OpenCV](http://opencv.org/)
- [Pylon](https://docs.baslerweb.com/software-installation-(linux))

## Build
Build Pylon grab example using CMake:
```bash
mkdir build
cd build
# [linux]
cmake ..
make -j$(nproc)
```

### Run example
To run the Pylon grab example, run the following commands:
```bash
cd build/
./grab
