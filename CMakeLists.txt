project(cameracalibration)
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
add_executable(cameracalibration main.cpp)
target_link_libraries(cameracalibration ${OpenCV_LIBS})

install(TARGETS cameracalibration RUNTIME DESTINATION bin)
