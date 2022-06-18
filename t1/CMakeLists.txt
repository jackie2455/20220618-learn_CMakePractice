project(HELLO)

set(SRC_LIST main.cpp)
message(STATUS "This is BINARY dir " ${HELLO_BINARY_DIR})
message(STATUS "This is SOURCE dir " ${HELLO_SOURCE_DIR})
message(STATUS "THis is PROJECT BINANR dir" ${PROJECT_BINARY_DIR})
message(STATUS "THIS is PROJECT SOURCE dir" ${PROJECT_SOURCE_DIR})

add_executable(hello ${SRC_LIST})

