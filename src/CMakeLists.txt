set(GTEST_ROOT $ENV{HOME}/work/googletest)
include_directories(
    ${GTEST_ROOT}/googletest/include
    )
add_Library(Add add.cpp)
