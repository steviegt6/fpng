set(LIBFPNG_SRCS fpng.cpp)

set(LIBFPNG_HDRS fpng.h)

add_library(libfpng SHARED ${LIBFPNG_HDRS} ${LIBFPNG_SRCS})

# Modify target properties so it links against libdeflate instead of deflate
set_target_properties(
    libdeflate_shared PROPERTIES
    OUTPUT_NAME libdeflate
    PUBLIC_HEADER libdeflate.h
    C_VISIBILITY_PRESET hidden
    SOVERSION 0
)

target_link_libraries(libfpng libdeflate::libdeflate_shared)