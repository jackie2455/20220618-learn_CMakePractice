project(HELLO)

set(SRC_LIST main.cpp)
add_executable(hello ${SRC_LIST})

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
set(LIBRARY_OUTPUT_PATH ${PROJECT_BIANRY_DIR}/lib)

message(STATUS "binary: ${PROJECT_BINARY_DIR}")
message(STATUS "source: ${PROJECT_SOURCE_DIR}")
