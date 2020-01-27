cmake_minimum_required(VERSION "3.16.3")

project("HelloWorld")  #$ give the project a name "HelloWorld" 

add_executable( "${PROJECT_NAME}" "Main.cpp")

install(TARGETS "${PROJECT_NAME}" DESTINATION bin) #${CMAKE_INSTALL_PREFIX}/bin
install(FILES "Main.cpp" DESTINATION src)          #${CMAKE_INSTALL_PREFIX}/bin 
