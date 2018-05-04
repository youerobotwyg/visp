project(tutorial-image)
cmake_minimum_required(VERSION 2.8)
find_package(VISP REQUIRED)
include_directories(${VISP_INCLUDE_DIRS})

add_executable(pose-from-qrcode-image pose-from-qrcode-image.cpp)
target_link_libraries(pose-from-qrcode-image ${VISP_LIBRARIES})
