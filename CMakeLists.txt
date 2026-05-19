cmake_minimum_required(VERSION 3.16)

if(CMAKE_CURRENT_SOURCE_DIR STREQUAL CMAKE_SOURCE_DIR)
    project(i2c_eeprom CXX)
endif()

add_library(i2c_eeprom STATIC
    "${CMAKE_CURRENT_SOURCE_DIR}/src/I2C_eeprom.cpp"
)
target_include_directories(i2c_eeprom PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")
