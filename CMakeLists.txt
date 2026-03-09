
cmake_minimum_required(VERSION 3.5)

FILE(GLOB_RECURSE app_sources src/*.*)

idf_component_register(SRCS ${app_sources}
                       INCLUDE_DIRS "include"
			REQUIRES arduino-esp32
)

project(PNGenc)
