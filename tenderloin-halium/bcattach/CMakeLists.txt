set(SOURCES
    hciattach.c
    hciattach_ti.c
    hciattach_st.c
    hciattach_tialt.c
    bluetooth.c
    hci.c)

add_executable(bcattach main.c)
add_executable(hciattach_awesome ${SOURCES})

install(
    TARGETS bcattach hciattach_awesome
    RUNTIME DESTINATION sbin
)
