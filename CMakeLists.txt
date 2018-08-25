cmake_minimum_required(VERSION 3.0)
project(dylibbundler)

add_executable(dylibbundler src/Dependency.cpp src/DylibBundler.cpp src/main.cpp src/Settings.cpp src/Utils.cpp)
target_include_directories(dylibbundler PRIVATE src)
install(TARGETS dylibbundler RUNTIME DESTINATION bin)
