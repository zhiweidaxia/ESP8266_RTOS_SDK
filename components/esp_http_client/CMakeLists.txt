set(COMPONENT_SRCS "esp_http_client.c"
                   "lib/http_auth.c"
                   "lib/http_header.c"
                   "lib/http_utils.c")
set(COMPONENT_ADD_INCLUDEDIRS "include")
set(COMPONENT_PRIV_INCLUDEDIRS "lib/include")

set(COMPONENT_REQUIRES "http_parser")
set(COMPONENT_PRIV_REQUIRES "mbedtls" "lwip" "esp-tls" "tcp_transport" "tcpip_adapter")

register_component()
