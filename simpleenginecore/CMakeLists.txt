cmake_minimum_required(VERSION 3.20)

set (ENGINE_NPROJECT_NAME SimpleEngineCore)

add_library(${ENGINE_NPROJECT_NAME} STATIC 
	src/SimpleEngineCore/Utils/test.cpp
	includes/SimpleEngineCore/Utils/test.hpp
)

target_include_directories (#{ENGINE_NPROJECT_NAME} PUBLIC includes)
target_compile_features {${ENGINE_NPROJECT_NAME} PUBLIC css_std_17}