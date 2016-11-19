cmake_minimum_required(VERSION 2.8)
set(GTEST_ROOT $ENV{HOME}/work/googletest)

include_directories(
    ${GTEST_ROOT}/googletest/include
    )

add_executable(test1 test_add.cpp)
target_link_libraries(test1
    Add
    pthread 
    ${GTEST_ROOT}/build/googlemock/libgmock.a
    ${GTEST_ROOT}/build/googlemock/libgmock_main.a
    )

