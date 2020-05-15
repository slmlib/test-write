cmake_minimum_required(VERSION 3.0)

project(slm-test-write
    DESCRIPTION "slm test write"
)

add_compile_definitions(
    SLM_EXPORT
)

add_library(slm-test-write SHARED
    slm-test-write.cpp
)

set_target_properties(slm-test-write PROPERTIES
    PUBLIC_HEADER slm-test-write.hpp
)
