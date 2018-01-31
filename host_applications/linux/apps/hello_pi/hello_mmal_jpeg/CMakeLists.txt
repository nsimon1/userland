set(EXEC hello_mmal_jpeg.bin)
set(SRCS jpeg.c)

add_executable(${EXEC} ${SRCS})
target_link_libraries(${EXEC} ${HELLO_PI_MMAL_LIBS})

install(TARGETS ${EXEC}
        RUNTIME DESTINATION bin)
