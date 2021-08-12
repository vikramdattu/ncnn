# Nanodet model running on ESP32

nanodet is well known tiny object detection model. This example runs the nanodet example with ncnn platform on ESP chips.
## How to use example

Follow detailed instructions provided specifically for this example.

Select the instructions depending on Espressif chip installed on your development board:

- [ESP32 Getting Started Guide](https://docs.espressif.com/projects/esp-idf/en/stable/get-started/index.html)
- [ESP32-S2 Getting Started Guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s2/get-started/index.html)


## Example folder contents

The project **nanodet** contains one source file in cpp language [nanodet_main.cpp](main/nanodet_main.c). The file is located in folder [main](main).

ESP-IDF projects are built using CMake. The project build configuration is contained in `CMakeLists.txt` files that provide set of directives and instructions describing the project's source files and targets (executable, library, or both).

Below is short explanation of remaining files in the project folder.

```
├── CMakeLists.txt
├── main
│   ├── CMakeLists.txt
│   ├── nanodet_m.bin
│   ├── nanodet_m.param
│   └── nanodet_main.c
├── CMakeList.txt              CMakeList to generate example
└── README.md                  This is the file you are currently reading
```

The example also uses `ncnn` library placed in [esp/ncnn](../esp/ncnn) directory.

For more information on structure and contents of ESP-IDF projects, please refer to Section [Build System](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-guides/build-system.html) of the ESP-IDF Programming Guide.
