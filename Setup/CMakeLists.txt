project(SetupTest)

enable_testing()
find_package(GTest)

set( Test_SRCS
    main.cpp
)

include_directories(${GTEST_ROOT}/include)

add_executable(SetupTest ${Test_SRCS})
target_link_libraries(SetupTest GTest::GTest GTest::Main)

