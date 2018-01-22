project(qcommon)

file(GLOB SOURCES_qcommon "*.c")

add_library(
    qcommon 
    ${SOURCES_qcommon}
    )

target_link_libraries(
    qcommon 
    winmm
    wsock32
    )