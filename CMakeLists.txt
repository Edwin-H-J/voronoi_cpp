cmake_minimum_required(VERSION 3.26)
set(PROJECT_NAME VoronoiCpp)
project(VoronoiCpp)

add_subdirectory(3rd/mathfu)

add_executable(${PROJECT_NAME} src/main.cpp)

mathfu_configure_flags(${PROJECT_NAME})
# target_include_directories(${PROJECT_NAME} PRIVATE 3rd/mathfu/include)