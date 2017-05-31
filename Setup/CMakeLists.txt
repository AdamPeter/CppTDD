project(SetupTest)

enable_testing()
find_package(GTest)
set( Test_SRCS
    main.cpp
)

set( Test_LIBS
    libgmock.a
    libgmock_main.a
)

add_executable(SetupTest ${Test_SRCS})
target_link_libraries(SetupTest GTest::GTest GTest::Main ${Test_LIBS})

