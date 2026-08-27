cmake_minimum_required(VERSION 3.10.2)
project(imgui_android_lib)

set(CMAKE_CXX_STANDARD 17)

add_library(
    imgui_android_lib
    SHARED
    main.cpp
    imgui.cpp
    imgui_demo.cpp
    imgui_draw.cpp
    imgui_tables.cpp
    imgui_widgets.cpp
    imgui_impl_android.cpp
    imgui_impl_opengl3.cpp
)

target_link_libraries(
    imgui_android_lib
    EGL
    GLESv3
    android
    log
)
