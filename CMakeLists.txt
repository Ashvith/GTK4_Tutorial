cmake_minimum_required(VERSION 3.20)
project(GTK4_Tutorial)

set(CMAKE_CXX_STANDARD 20)
set(FILES "pr1" "pr2" "pr3" "pr4" "lb1" "lb2" "lb3")

find_package(PkgConfig REQUIRED)
pkg_check_modules(GTK4 REQUIRED gtk4)

include_directories(${GTK4_INCLUDE_DIRS})
link_directories(${GTK4_LIBRARY_DIRS})
add_definitions(${GTK4_CFLAGS_OTHER})

foreach(LETTER ${FILES})
add_executable(${LETTER} ${LETTER}.c)
  target_link_libraries(${LETTER} ${GTK4_LIBRARIES})
endforeach()