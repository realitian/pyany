
PYTHON_ADD_MODULE(Test Test.cpp)
ADD_EXECUTABLE(TestApp Test.cpp)
TARGET_LINK_LIBRARIES(Test ${Boost_LIBRARIES} ${PYTHON_LIBRARIES})
FILE(COPY Test.py DESTINATION .)
ADD_TEST(TestAny Test.py)
