cmake_minimum_required(VERSION 3.13)
set(CMAKE_VERBOSE_MAKEFILE on)

file(GLOB rnoh_card_view_SRC CONFIGURE_DEPENDS *.cpp)
add_library(rnoh_card_view SHARED ${rnoh_card_view_SRC})

target_include_directories(rnoh_card_view PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(rnoh_card_view PUBLIC rnoh)


