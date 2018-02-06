add_executable(rfcomm-client
    rfcomm-client.cpp
)
#target_include_directories(rfcomm-client PUBLIC )
target_link_libraries(rfcomm-client bluetooth)

add_executable(rfcomm-server
	rfcomm-server.cpp
)
#target_include_directories(rfcomm-server PUBLIC )
target_link_libraries(rfcomm-server bluetooth)