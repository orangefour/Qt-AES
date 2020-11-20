find_package(Qt5 COMPONENTS Core REQUIRED)

add_library(QtAES qaesencryption.cpp)
target_include_directories(QtAES PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(QtAES Qt::Core)
