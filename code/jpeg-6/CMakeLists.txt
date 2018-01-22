project(jpeg6)

file(GLOB jpeg6_SOURCES "*.c")

add_library(jpeg6
    ${jpeg6_SOURCES}
    )

target_link_libraries(
    jpeg6 
    winmm
    wsock32
    )