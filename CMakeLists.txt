cmake_minimum_required(VERSION 2.8)
add_subdirectory(src)
set(GTEST_ROOT $ENV{HOME}/work/googletest)
include_directories(
    ${GTEST_ROOT}/googletest/include
    )
add_executable(test1 src/test1.cpp)
target_link_libraries(test1 pthread 
    ${GTEST_ROOT}/build/googlemock/libgmock.a
    ${GTEST_ROOT}/build/googlemock/libgmock_main.a
    )

