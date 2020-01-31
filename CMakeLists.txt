
add_library(freetype-gl STATIC "platform.c" "texture-atlas.c" "texture-font.c" "vector.c" "utf8-utils.c" "distance-field.c" "edtaa3func.c")

target_include_directories(freetype-gl PRIVATE "../freetype/include")

target_link_libraries(freetype-gl PRIVATE freetype)
