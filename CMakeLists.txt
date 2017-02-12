cmake_minimum_required (VERSION 2.6)
project (paravia)


# link in curses
find_package(Curses REQUIRED)
include_directories(${CURSES_INCLUDE_DIR})

add_executable(paravia paravia.c)
set_property(TARGET paravia PROPERTY C_STANDARD 99)
target_link_libraries(paravia ${CURSES_LIBRARIES})







#############3
#cmake_minimum_required(VERSION 2.4.6)
#
##set the default path for built executables to the "bin" directory
#set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
##set the default path for built libraries to the "lib" directory
#set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)
#
##For the Curses library to load:
#SET(CURSES_USE_NCURSES TRUE)
#
#include_directories(
#     "src/"
#)
#add_subdirectory(src)