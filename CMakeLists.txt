
cmake_minimum_required(VERSION 3.16)

# Incluyendo el archivo project.cmake del entorno ESP-IDF.
include($ENV{IDF_PATH}/tools/cmake/project.cmake)
project(SistemaRiegoAI)

# Definimos los directorios adicionales donde se encuentran los componentes.
set(EXTRA_COMPONENT_DIRS 
    "C:/Espressif/projects/SistemaRiegoAI/SistemaRiegoAI/components/ESP32_LoRaWAN-master/src"
    "C:/Espressif/projects/SistemaRiegoAI/SistemaRiegoAI/components/Heltec_ESP32-master/src"
    "C:/Espressif/projects/SistemaRiegoAI/SistemaRiegoAI/components/WiFi_Kit_series-master/cores"
    "C:/Espressif/projects/SistemaRiegoAI/SistemaRiegoAI/components/arduino"
    "C:/Espressif/projects/SistemaRiegoAI/SistemaRiegoAI/components/arduino-esp32")

set(ENV{ARDUINO_SKIP_IDF_VERSION_CHECK} "1")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wno-error=all")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wno-error=all")

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -O0")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O0")
