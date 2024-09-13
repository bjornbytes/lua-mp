cmake_minimum_required(VERSION 3.5.0)
project(lua-mp)

add_library(lua-mp MODULE mp.c)
set_target_properties(lua-mp PROPERTIES WINDOWS_EXPORT_ALL_SYMBOLS TRUE)
set_target_properties(lua-mp PROPERTIES POSITION_INDEPENDENT_CODE TRUE)
set_target_properties(lua-mp PROPERTIES PREFIX "")
set_target_properties(lua-mp PROPERTIES OUTPUT_NAME "mp")
