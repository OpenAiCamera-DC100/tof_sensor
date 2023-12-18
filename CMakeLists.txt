cmake_minimum_required(VERSION 3.8)

project(tof_sensor)

set(VZENSE_TOF_LIB
    ${CMAKE_SOURCE_DIR}/lib/libImgPreProcess.so
    ${CMAKE_SOURCE_DIR}/lib/libvzense_api.so
    ${CMAKE_SOURCE_DIR}/lib/libvzense_api.so.3.5
    ${CMAKE_SOURCE_DIR}/lib/libvzense_api.so.3.5.4
)

install(FILES ${VZENSE_TOF_LIB} DESTINATION lib)
install(DIRECTORY ${CMAKE_SOURCE_DIR}/include/ DESTINATION "include")
