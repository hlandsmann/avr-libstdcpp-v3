add_library(avr-stdcpp-v3 INTERFACE)
add_library(std-avr::std-avr ALIAS avr-stdcpp-v3)

target_include_directories(avr-stdcpp-v3
    INTERFACE
        include
)

target_compile_features(avr-stdcpp-v3 INTERFACE cxx_std_20)
