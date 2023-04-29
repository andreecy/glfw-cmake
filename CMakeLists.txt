cmake_minimum_required(VERSION 3.0.0)
project(new_project VERSION 0.1.0)

file(GLOB TARGET_SRC 
"src/*.cpp"
)

add_executable(main ${TARGET_SRC})

add_subdirectory("lib")
target_link_libraries(main glfw glad)