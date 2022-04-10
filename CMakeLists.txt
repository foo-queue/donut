cmake_minimum_required(VERSION 3.0.0)
project(donut VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(donut donut.cpp)
target_compile_features(donut PUBLIC cxx_std_20)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
