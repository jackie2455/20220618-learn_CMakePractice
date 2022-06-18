cmake_minimum_required(VERSION 3.18)
project(HELLO)

message(STATUS "THis is PROJECT BINANR dir" ${PROJECT_BINARY_DIR})
message(STATUS "THIS is PROJECT SOURCE dir" ${PROJECT_SOURCE_DIR})

#add_subdirectory(src bin)
add_subdirectory(src)

install(FILES COPYRIGHT README DESTINATION share/doc/cmake/t2)
install(TARGETS hello RUNTIME DESTINATION bin)
install(PROGRAMS runhello.sh DESTINATION bin)
install(DIRECTORY doc/ DESTINATION share/doc/cmake/t2)

