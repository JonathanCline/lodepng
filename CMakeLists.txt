add_library(lodepng STATIC
    "lodepng.cpp")
target_include_directories(lodepng PUBLIC "${CMAKE_CURRENT_LIST_DIR}")


if(MSVC)
    target_compile_options(lodepng PRIVATE /wd4334 /wd4267 /wd6297 /wd6011)
endif()
