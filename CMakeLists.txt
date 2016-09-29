cmake_minimum_required(VERSION 3.3)

project(boost_assert)

add_library(boost_assert INTERFACE)

target_include_directories(boost_assert BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_assert DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
