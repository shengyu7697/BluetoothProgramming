add_executable(simplescan
    simplescan.cpp
)

#target_include_directories(simplescan PUBLIC )
target_link_libraries(simplescan bluetooth)