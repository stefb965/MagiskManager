cmake_minimum_required(VERSION 3.6)
add_library(zipadjust SHARED src/main/jni/zipadjust.c)
find_library(libz z)
find_library(liblog log)
target_link_libraries(zipadjust ${libz} ${liblog})