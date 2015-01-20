cmake_minimum_required(VERSION 2.8)

project(SFML_TEST_CMAKE)

add_executable(main main.cpp)

SET(LIBRARY_OUTPUT_PATH ${CMAKE_CURRENT_SOURCE_DIR}/lib)

SET(EXECUTABLE_OUTPUT_PATH ${CMAKE_CURRENT_SOURCE_DIR}/bin)

LINK_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR}/lib)

TARGET_LINK_LIBRARIES(main sfml-window sfml-graphics sfml-system)
