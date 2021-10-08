add_library(${PROJECT_NAME}_client STATIC oscs_client.c)
target_include_directories(${PROJECT_NAME}_client PUBLIC ../include)

add_library(${PROJECT_NAME}_server STATIC oscs_server.c)
target_include_directories(${PROJECT_NAME}_server PUBLIC ../include)
