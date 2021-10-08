add_executable(${PROJECT_NAME}_clientexec client.c)
target_link_libraries(${PROJECT_NAME}_clientexec PUBLIC ${PROJECT_NAME}_client)
set_target_properties(${PROJECT_NAME}_clientexec PROPERTIES RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")

add_executable(${PROJECT_NAME}_serverexec server.c)
target_link_libraries(${PROJECT_NAME}_serverexec PUBLIC ${PROJECT_NAME}_server)
set_target_properties(${PROJECT_NAME}_serverexec PROPERTIES RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")
