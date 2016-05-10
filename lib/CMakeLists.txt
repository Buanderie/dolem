project (LIBDOLEM)

include_directories(${LIBDOLEM_SOURCE_DIR}/include)

file (GLOB_RECURSE SRC_CPP ${LIBDOLEM_SOURCE_DIR}/*.c*)
add_library(dolem SHARED ${SRC_CPP})
