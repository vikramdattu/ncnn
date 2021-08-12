# This file is added to create an IDF component out of generated lib using procedure from `build.sh`
idf_component_register(INCLUDE_DIRS "include")

if(CONFIG_IDF_TARGET_ESP32S3)
add_prebuilt_library(ncnn ${COMPONENT_DIR}/lib/libncnn_esp32s3.a)
endif()
if(CONFIG_IDF_TARGET_ESP32)
add_prebuilt_library(ncnn ${COMPONENT_DIR}/lib/libncnn_esp32.a)
endif()
target_link_libraries(${COMPONENT_LIB} INTERFACE ncnn)
