set(SUB_NAME  "ano-protocol")

aux_source_directory(./source                                                         ${SUB_NAME}_SRC)

add_library( ${SUB_NAME} STATIC
    ${${SUB_NAME}_SRC}
)
target_include_directories( ${SUB_NAME} 
    PUBLIC 
        ./
)

