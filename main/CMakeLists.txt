cmake_minimum_required(VERSION 3.16)

# Ruta donde se encuentran los componentes del proyecto
set(EXTRA_COMPONENT_DIRS "C:/Espressif/projects/SistemaRiegoAI/SistemaRiegoAI/components")

# Agregar el componente principal del proyecto
idf_component_register(
    SRCS "hello_world_main.c"
    INCLUDE_DIRS "." "../components/ESP32_LoRaWAN-master/src" "../components/Heltec_ESP32-master/src" "../components/WiFi_Kit_series-master/cores"
    REQUIRES arduino
)
