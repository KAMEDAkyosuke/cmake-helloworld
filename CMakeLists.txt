cmake_minimum_required(VERSION 2.8)

project(cmake-helloworld)

add_subdirectory(subdir)

link_directories (${PROJECT_SOURCE_DIR}/subdir) 

add_executable(helloworld helloworld.c)

target_link_libraries(helloworld subdir)
