set(GTEST_ROOT $ENV{HOME}/work/googletest)
include_directories(
    ${GTEST_ROOT}/googletest/include
    )
add_Library(Test1 test1.cpp)
