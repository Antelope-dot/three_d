cmake_minimum_required(VERSION 3.20)
project(three_d)
set(EXECUTABLE_OUTPUT_PATH "out")

find_package(OpenGL REQUIRED)

add_executable(three_d 
	src/main.cpp 
	libraries/glad.h 
	libraries/glad.c
	)

target_link_libraries(three_d 
	glfw
	OpenGL::GL
	)
