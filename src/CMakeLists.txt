file(GLOB src *)
# copy runtime depedencies to build dir
add_custom_target(
    tech_params
    ${CMAKE_COMMAND} -E copy_directory ${CMAKE_SOURCE_DIR}/tech_params/ ${CMAKE_BINARY_DIR}/tech_params
)
add_executable(cacti ${src})

add_dependencies(cacti tech_params)
