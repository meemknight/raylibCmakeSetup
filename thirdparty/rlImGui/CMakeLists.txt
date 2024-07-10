cmake_minimum_required(VERSION 3.1)
project(rlimgui)

add_library(rlimgui)
target_sources(rlimgui PRIVATE "rlImGui.cpp" "rlImGui.h")
target_include_directories(rlimgui PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/")
target_link_libraries(rlimgui PUBLIC imgui raylib_static)