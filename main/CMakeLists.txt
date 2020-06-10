idf_component_register(SRCS "Capsense.cpp" "data.cpp" "fs_json.cpp" "IMU.cpp" "libmapper.cpp" "main.cpp" "OSC.cpp" "WiFi.cpp" "instrument.cpp"
                       INCLUDE_DIRS "./"
                       REQUIRES arduino-esp32 TStick-arduino-libraries libmapper-idf)
target_compile_options(${COMPONENT_LIB} PRIVATE -DESP32 -Wno-format)
