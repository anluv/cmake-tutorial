cmake_minimum_required(VERSION 3.16.0)

project(Tutorial VERSION 1.0)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)
configure_file(TutorialConfig.h.in TutorialConfig.h @ONLY)
add_executable(${PROJECT_NAME} tutorial.cxx)
target_include_directories(${PROJECT_NAME} PUBLIC ${PROJECT_BINARY_DIR})

