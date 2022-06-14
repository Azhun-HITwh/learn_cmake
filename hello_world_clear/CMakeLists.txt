cmake_minimum_required(VERSION 3.0.0)

project(hello)

add_subdirectory(src)

INSTALL(FILES COPYRIGHT README.md DESTINATION share/doc/cmake/hello-world-clear)

INSTALL(PROGRAMS runhello.sh DESTINATION bin)

INSTALL(DIRECTORY doc/ DESTINATION share/doc/cmake/hello-world-clear/doc)

INSTALL(DIRECTORY demo/ DESTINATION share/doc/cmake/hello-world-clear/demo)
