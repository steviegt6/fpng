cmake_minimum_required(VERSION 3.5) # < 3.5 compatibility deprecated
set(CMAKE_CXX_STANDARD 20)

project(fpng VERSION 1.0.0 LANGUAGES CXX)
set(CMAKE_EXPORT_COMPILE_CMMANDS ON CACHE INTERNAL "")

# Add libraries
add_subdirectory(lib)

# Add source projects
add_subdirectory(src)

message("[${PROJECT_NAME}] Compiler is " ${CMAKE_CXX_COMPILER_ID} " " ${CMAKE_CXX_COMPILER_VERSION} " on " ${CMAKE_SYSTEM_NAME} " " ${CMAKE_SYSTEM_VERSION})
