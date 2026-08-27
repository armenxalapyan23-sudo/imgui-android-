cmake_minimum_required(VERSION 3.10.0)
project(imgui_android_lib)

add_library(imgui_android_lib SHARED 
    main.cpp 
    imgui.cpp 
    imgui_draw.cpp 
    imgui_tables.cpp 
    imgui_widgets.cpp 
    backends/imgui_impl_android.cpp
)

target_include_directories(imgui_android_lib PRIVATE . backends)
