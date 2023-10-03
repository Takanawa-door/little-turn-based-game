cmake_minimum_required (VERSION 3.23)

set (CMAKE_CXX_STANDARD 20)
set (CMAKE_CXX_STANDARD_REQUIRED true)
set (CMAKE_EXPORT_COMPILE_COMMANDS true)
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -static")

project (theLittleTurnBasedGame)

include_directories (./include)
aux_source_directory (./src/ltbgame SRC)

add_executable (theLittleTurnBasedGame ${SRC})
