
# Let us add unit testing for the rock_paper_scissor library
add_executable(test_rock_paper_scissor test_rock_paper_scissor.c)
# We need to link both with the library we are testing and the mtest framework.
target_link_libraries(test_rock_paper_scissor rock_paper_scissor mtest)

# Add test cases to CTest (our test framework has a nice macro for that).
discover_tests(test_rock_paper_scissor)
