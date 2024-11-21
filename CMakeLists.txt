cmake_minimum_required(VERSION 3.21)

project(canteen)

macro(add_meals)
	foreach(meal ${ARGN})
		add_subdirectory(meal/cango.${meal})
	endforeach()
endmacro()

macro(add_raw)
	foreach(raw ${ARGN})
		add_subdirectory(raw/cango.${raw})
	endforeach()
endmacro()
