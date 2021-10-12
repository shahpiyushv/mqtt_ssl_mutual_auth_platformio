# This file was automatically generated for projects
# without default 'CMakeLists.txt' file.

FILE(GLOB_RECURSE app_sources ${CMAKE_SOURCE_DIR}/src/*.c)

idf_component_register(SRCS ${app_sources})
target_add_binary_data(${COMPONENT_TARGET} "client.crt" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "client.key" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "server.crt" TEXT)

