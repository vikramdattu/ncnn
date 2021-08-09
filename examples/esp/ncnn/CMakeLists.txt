# This file is added to create an IDF component out of generated lib using procedure from `build.sh`
idf_component_register(INCLUDE_DIRS "include")

add_prebuilt_library(ncnn ${COMPONENT_DIR}/lib/libncnn.a)
target_link_libraries(${COMPONENT_LIB} INTERFACE ncnn)
