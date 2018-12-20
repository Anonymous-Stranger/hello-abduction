
cmake_minimum_required(VERSION 2.8)

project(HelloAbduction)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY bin)

add_subdirectory(ext/mistral)

include_directories(
	include
	src
  ${MISTRAL_INCLUDE_DIRS}
)

add_executable(HelloAbduction
	src/__main.cpp
)

target_link_libraries(HelloAbduction
	mistral
  gmp
)
