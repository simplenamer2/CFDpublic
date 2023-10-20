cmake_minimum_required(VERSION 3.0)

project(cfd_tests)

set(EXE cfd_test.cpp)

include_directories(matcsr)
add_executable(cfd_test ${EXE})
add_subdirectory(matcsr)

target_link_libraries(cfd_test matcsr)
