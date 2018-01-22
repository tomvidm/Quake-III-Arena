file(GLOB SOURCES_WIN32 "${CMAKE_CURRENT_SOURCE_DIR}/win32/*.c")

project(game)

add_subdirectory(client)
#add_subdirectory(jpeg-6)
add_subdirectory(qcommon)
add_subdirectory(renderer)

#[[
add_executable(
    win32
    ${SOURCES_WIN32}
)

target_link_libraries(win32
    winmm
    wsock32
)
]]