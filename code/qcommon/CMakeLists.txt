project(qcommon)

set(qcommon_COMMON_SOURCES
    cm_load.c
    cm_patch.c
    cm_polylib.c
    cm_test.c
    cm_trace.c
    cmd.c
    common.c
    cvar.c
    files.c
    huffman.c
    md4.c
    msg.c
    net_chan.c
    unzip.c
    vm.c
    vm_interpreted.c
    vm_x86.c
    )   

add_library(
    qcommon
    ${qcommon_COMMON_SOURCES}
    )

target_link_libraries(
    qcommon 
    winmm
    wsock32
    )