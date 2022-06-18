project(NEWHELLO)

set(SRC_LIST main.cpp)
set(HELLO_INCLUDE_DIR "/tmp/usr/t3/include/hello")
set(HELLO_LIB_DIR "/tmp/usr/t3/lib/libhello.so")

include_directories(${HELLO_INCLUDE_DIR})
#link_directories("/tmp/usr/t3/lib")


add_executable(newhello ${SRC_LIST})
target_link_libraries(newhello ${HELLO_LIB_DIR})
#target_link_libraries(newhello libhello.so)


