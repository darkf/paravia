cmake_minimum_required (VERSION 2.6)
project (paravia)

add_executable(paravia paravia.c)
set_property(TARGET paravia PROPERTY C_STANDARD 99)
target_link_libraries(paravia)
