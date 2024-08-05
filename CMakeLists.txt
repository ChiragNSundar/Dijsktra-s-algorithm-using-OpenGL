cmake_minimum_required(VERSION 3.28)
project(lab)

find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)

set(CMAKE_CXX_STANDARD 17)

add_executable(lab main.cpp
)
target_link_libraries(lab ${OPENGL_LIBRARIES})
target_link_libraries(lab ${GLUT_LIBRARIES})