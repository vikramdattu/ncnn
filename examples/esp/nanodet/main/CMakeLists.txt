
idf_component_register(SRCS "nanodet_main.cpp"
                       EMBED_TXTFILES nanodet_m.bin nanodet_m.param
                       PRIV_REQUIRES ncnn)
