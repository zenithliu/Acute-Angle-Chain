file(GLOB HEADERS "include/aacio/chain_plugin/*.hpp")
add_library( chain_plugin
             chain_plugin.cpp
             ${HEADERS} )

target_link_libraries( chain_plugin aacio_chain appbase )
target_include_directories( chain_plugin PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include" )
