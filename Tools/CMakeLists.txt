file(GLOB_RECURSE srcs CONFIGURE_DEPENDS src/*.c include/*.h)
set(ROOT_DIR ${CMAKE_CURRENT_LIST_DIR}/..)
add_library(Tools STATIC ${srcs})
add_subdirectory(${ROOT_DIR}/DS Tools_DS_binnary_dir)
target_include_directories(Tools PUBLIC include)
target_link_libraries(Tools PRIVATE DS)
# target_link_libraries(Tools PUBLIC DS)