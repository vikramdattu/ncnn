
idf_component_register(SRCS "nanodet_main.cpp"
                       EMBED_TXTFILES nanodet_m.bin nanodet_m.param image0.rgb image1.rgb image2.rgb
                       PRIV_REQUIRES ncnn)
