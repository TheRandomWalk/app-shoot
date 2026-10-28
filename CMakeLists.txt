cmake_minimum_required(VERSION 3.20)
project(AppShoot LANGUAGES CXX)

add_executable(AppShoot main.cpp)
target_compile_features(AppShoot PRIVATE cxx_std_20)
target_compile_definitions(AppShoot PRIVATE UNICODE _UNICODE WIN32_LEAN_AND_MEAN NOMINMAX)
target_link_libraries(AppShoot PRIVATE gdiplus dwmapi user32 gdi32)
