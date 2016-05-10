cmake_minimum_required(VERSION 2.8)
project(DOLEM_EXAMPLE0)

include_directories(${LIBDOLEM_SOURCE_DIR}/include)

# Add libmagog
LINK_DIRECTORIES(${LIBDOLEM_BINARY_DIR})
set( DEPS "${DEPS};dolem" )

# Global shit
file (GLOB_RECURSE FILES_CPP ./*.c*)
add_executable(dolem_example0 ${FILES_CPP})

target_link_libraries (dolem_example0 ${DEPS} )
