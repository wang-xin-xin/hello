cmake_minimum_required(VERSION 3.13)
project(app)

set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_C_EXTENSIONS OFF)
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

# set(CMAKE_BUILD_TYPE Debug)
# set(CMAKE_BUILD_TYPE RelWithDebInfo)
set(CMAKE_BUILD_TYPE Release)

# add_executable(hr_sum_array hr_sum_array.cpp)
add_executable(lambda lambda.cpp)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/../../boost/include/boost-1_69)
link_libraries(${CMAKE_CURRENT_SOURCE_DIR}/../../boost/lib)
