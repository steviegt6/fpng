# project(test)

set(TEST_SRCS fpng_test.cpp lodepng.cpp pvpngreader.cpp)

set(TEST_HDRS)

include_directories(${LIBFPNG_INCLUDE})

add_executable(test ${TEST_HDRS} ${TEST_SRCS})

target_link_libraries(test libfpng)