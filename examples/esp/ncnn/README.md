### What is this lib?

- This component is created using steps for ESP32 given in build.sh file and adding CMakeList.txt to register this as component.
- I am not convinced with the location of the lib in `examples`, but it is convenient for now.

- Run the following commands in ncnn directory to build and create the same.

```
mkdir -p build-esp32
pushd build-esp32
cmake -DCMAKE_TOOLCHAIN_FILE=../toolchains/esp32.toolchain.cmake -DNCNN_OPENMP=OFF -DNCNN_THREADS=OFF -DNCNN_RUNTIME_CPU=OFF -DNCNN_SIMPLEOCV=ON -DNCNN_BUILD_BENCHMARK=OFF -DNCNN_STDIO=OFF ..
make -j4
make install
popd
```

- Take a look at `examples/esp/` for examples for ESP platforms.
