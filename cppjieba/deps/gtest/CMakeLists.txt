INCLUDE_DIRECTORIES(./ include)
ADD_LIBRARY(gtest STATIC src/gtest-all.cc)
if(NOT MSVC)
	TARGET_LINK_LIBRARIES(gtest pthread)
endif()
