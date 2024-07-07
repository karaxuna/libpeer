file(GLOB SOURCES_C "./src/*.c")

idf_component_register(
  SRCS ${SOURCES_C}
  INCLUDE_DIRS "./src"
  REQUIRES mbedtls srtp2 mdns
)
