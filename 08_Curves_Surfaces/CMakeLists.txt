cmake_minimum_required(VERSION 3.15)
project(08_Curves_Surfaces)

set(CMAKE_CXX_STANDARD 11)

include_directories(include)
link_directories(lib)

aux_source_directory(src SRC)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/out)

add_executable(curve_editor ${SRC})
target_link_libraries(curve_editor freeglutd.lib)

