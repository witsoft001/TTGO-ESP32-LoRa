set(COMPONENT_ADD_INCLUDEDIRS .)

file(GLOB component_files "*.c")

set(COMPONENT_SRCS ${component_files})

set(COMPONENT_REQUIRES message)
set(COMPONENT_PRIV_REQUIRES nvs_flash wifi mqtt http)

register_component()
