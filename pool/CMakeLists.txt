add_definitions(-DMODULE=pool)

add_executable(pool main.cpp BlockTemplatePoller.cpp DaemonConnector.cpp Pool.cpp)
target_link_libraries(pool util socket stratum bitcoinrpc mining pthread)

