cmake_minimum_required(VERSION 3.15)
project(MVC-Example CXX C)

add_executable(
  MVC-Example MVC-Example.cpp src/Student.cpp src/StudentController.cpp
              src/StudentView.cpp src/StudentViewTwo.cpp)

target_include_directories(MVC-Example PUBLIC src)

install(
  TARGETS MVC-Example
  DESTINATION "."
  RUNTIME DESTINATION bin
  ARCHIVE DESTINATION lib
  LIBRARY DESTINATION lib)
