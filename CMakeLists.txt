find_package(Qt5 COMPONENTS Core REQUIRED)

file(GLOB SOURCES *.cpp)
add_library(QtAES ${LIB_TYPE} ${SOURCES})
target_include_directories(QtAES PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
qt5_use_modules(QtAES Core)
