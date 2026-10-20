
# Let us add unit testing for the test_planets library
add_executable(test_planets test_planets.c)
# We need to link both with the library we are testing and the mtest framework.
target_link_libraries(test_planets planets mtest)

# Add test cases to CTest (our test framework has a nice macro for that).
discover_tests(test_planets)
