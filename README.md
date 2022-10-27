## How to Build and Install
This project uses CMake to orchestrate the build and installallation process. To build and install on your host system, follow these easy steps:
1. `git clone https://github.com/DavidLeeds/hashmap.git` - download the source
2. `mkdir build-hashmap && cd build-hashmap` - create a build directory outside the source tree
3. `cmake ../hashmap` - run CMake to setup the build
4. `make` - compile the code
5. `make test` - run the unit tests (if enabled)
6. `sudo make install` - _OPTIONAL_ install the library on this system

##### CMake Options

* `HASHMAP_BUILD_TESTS` - Set to `ON` to generate unit tests.
* `HASHMAP_BUILD_EXAMPLES` - Set to `ON` to build example code. 

##### Put Performence
|  Type   | Runtime  |
|  ----  | ----  |
| No_Flush  | 77220ms |
| Flush_10  | 150176ms |
| Flush_500  | 351451ms |
| Flush_1000  | 561014ms |
