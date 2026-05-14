add_library(ImGui STATIC
    imgui.cpp
    imgui_draw.cpp
    imgui_tables.cpp
    imgui_widgets.cpp
    imgui_demo.cpp
)

target_include_directories(ImGui PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
set_target_properties(ImGui PROPERTIES
    CXX_STANDARD 17
    POSITION_INDEPENDENT_CODE ON
)
