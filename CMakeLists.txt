cmake_minimum_required(VERSION 3.21)
project(webserver)

set(CMAKE_CXX_STANDARD 98)

add_executable(webserver
        webserv_core/main.cpp
        webserv_core/config_parser/ConfigInfo.cpp
        webserv_core/config_parser/Location_info.cpp
        webserv_core/config_parser/ServerConfig.cpp
        webserv_core/config_parser/Utils_parse_config.cpp
        webserv_core/utils/Request.cpp
        webserv_core/sockets/BindingSocket.cpp
        webserv_core/sockets/ListeningSocket.cpp
        webserv_core/sockets/SimpleSocket.cpp
        webserv_core/servers/WebServer.cpp
        webserv_core/utils/CGI_handler.cpp
        webserv_core/utils/Request_handler.cpp
        webserv_core/utils/utils.cpp
        webserv_core/utils/Error_response_generator.cpp

        )