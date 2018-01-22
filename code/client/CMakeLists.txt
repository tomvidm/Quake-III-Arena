project(client)

file(GLOB client_SOURCES "*.c")

add_library(client
    ${client_SOURCES}
    )

target_link_libraries(
    client 
    winmm
    wsock32
    )