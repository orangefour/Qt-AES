find_package(Qt5 COMPONENTS Core REQUIRED)

add_library(QtAES ${LIB_TYPE} qaesencryption.cpp)
target_include_directories(QtAES PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
qt5_use_modules(QtAES Core)
