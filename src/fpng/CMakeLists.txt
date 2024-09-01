set(FPNG_SRCS main.cpp)

set(FPNG_HDRS)

include_directories(${LIBFPNG_INCLUDE})

add_executable(${PROJECT_NAME} ${FPNG_HDRS} ${FPNG_SRCS})