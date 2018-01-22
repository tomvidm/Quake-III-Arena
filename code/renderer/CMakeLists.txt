project(renderer)

file(GLOB renderer_SOURCES "*.c")

add_library(renderer
    ${renderer_SOURCES}
)