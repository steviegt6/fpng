set(LIBFPNG_SRCS fpng.cpp)

set(LIBFPNG_HDRS fpng.h)

add_library(libfpng ${LIBFPNG_HDRS} ${LIBFPNG_SRCS})

target_link_libraries(libfpng libdeflate::libdeflate_shared)