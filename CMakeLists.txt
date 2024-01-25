# CMakeLists.txt

cmake_minimum_required(VERSION 3.0)

project(HelloWorld)

set(CMAKE_SYSTEM_NAME Linux)
set(CMAKE_SYSTEM_PROCESSOR aarch64)

set(CMAKE_C_COMPILER /usr/bin/aarch64-linux-gnu-gcc)
set(CMAKE_CXX_COMPILER /usr/bin/aarch64-linux-gnu-g++)

# Replace the YOUR_SYSROOT_PATH with a valid sysroot of aarch64 linux system
SET(CMAKE_SYSROOT YOUR_SYSROOT_PATH)

add_executable(helloworld helloworld.c)

