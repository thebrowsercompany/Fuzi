cmake_minimum_required(VERSION 3.19.6)

project(Fuzi LANGUAGES Swift)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
set(CMAKE_Swift_MODULE_DIRECTORY ${CMAKE_BINARY_DIR}/swift)

# LibXml2 must be built 
add_subdirectory(Vendor)

add_subdirectory(Sources)
