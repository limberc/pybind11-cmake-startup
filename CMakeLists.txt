cmake_minimum_required(VERSION 3.15)
project(binder)

set(CMAKE_CXX_STANDARD 14)
add_subdirectory(pybind11)
set(PYBIND11_CPP_STANDARD -std=c++11)
pybind11_add_module(binder src/main.cpp)
