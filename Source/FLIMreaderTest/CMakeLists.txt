cmake_minimum_required(VERSION 3.0)

PROJECT(FLIMreaderTest)

cmake_policy(SET CMP0020 NEW)
cmake_policy(SET CMP0043 NEW)

include_directories(../FLIMreader)


# Source Files
#====================================
set(SOURCE
   FLIMreaderTest.cpp
)

set(HEADERS
   FLIMreaderTest.h
)

add_executable(FLIMreaderTest ${SOURCE} ${HEADERS} $<TARGET_OBJECTS:FLIMreader>)
