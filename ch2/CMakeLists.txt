project(ch2)

enable_testing()
find_package(GTest)
set( Test_SRCS
    main.cpp
    SoundexTests.cpp
)

set( Test_LIBS
    libgmock.a
    libgmock_main.a
)

add_executable(ch2 ${Test_SRCS})
target_link_libraries(ch2 GTest::GTest GTest::Main ${Test_LIBS})

