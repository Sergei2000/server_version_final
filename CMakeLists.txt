cmake_minimum_required(VERSION 3.14)
project(untitled1)

set(CMAKE_CXX_STANDARD 17)
find_package(Boost REQUIRED COMPONENTS system filesystem thread log log_setup)
add_executable(untitled1 main.cpp)
target_link_libraries(untitled1 ${Boost_LIBRARIES})
set (CMAKE_CXX_FLAGS "-g -Wall -DBOOST_LOG_DYN_LINK")
