project(screensaver.greynetic)

cmake_minimum_required(VERSION 2.6)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${PROJECT_SOURCE_DIR})

enable_language(CXX)

find_package(kodi REQUIRED)

include_directories(${KODI_INCLUDE_DIR})

set(GREYNETIC_SOURCES src/GreyNetic.cpp)

set(DEPLIBS)

build_addon(screensaver.greynetic GREYNETIC DEPLIBS)

include(CPack)
