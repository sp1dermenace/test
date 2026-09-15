cmake_minimum_required(VERSION 3.30)

set(PROJECT_NAME test)
file(GLOB PATH_STR "${CMAKE_CURRENT_SOURSE_DIR}/src/*.cpp" 
				  "${CMAKE_CURRENT_SOURCE_DIR}/src/*.hpp")
				  
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/src)
add_executable(${PROJECT_NAME} ${PATH_STR})