cmake_minimum_required(VERSION 3.1)

project(JCuda)

include(${CMAKE_CURRENT_SOURCE_DIR}/../jcuda-common/JCudaCommon_CMake.txt)

add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/src/main/native/cublas
    ${CMAKE_CURRENT_BINARY_DIR}/JCublas/JCublasJNI/bin)
    
add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/src/main/native/cublas2
    ${CMAKE_CURRENT_BINARY_DIR}/JCublas/JCublas2JNI/bin)
