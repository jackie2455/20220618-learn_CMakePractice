project(HELLOLIB)

set(LIBHELLO_LIST hello.cpp)
add_library(hello SHARED ${LIBHELLO_LIST})
add_library(hello_static STATIC ${LIBHELLO_LIST})

set_target_properties(hello_static PROPERTIES OUTPUT_NAME "hello")

install(TARGETS hello hello_static
	LIBRARY DESTINATION lib 
	ARCHIVE DESTINATION lib)
install(FILES hello.h DESTINATION include/hello)

