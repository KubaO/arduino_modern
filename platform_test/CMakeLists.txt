
generate_avr_firmware(standard
    SRCS standard.cpp
    PORT  /dev/ttyACM0
    SERIAL picocom @SERIAL_PORT@ -b 9600 -l
    BOARD uno)

    
generate_arduino_firmware(stepper
    SRCS stepper.cpp
    PORT  /dev/ttyACM0
    SERIAL picocom @SERIAL_PORT@ -b 9600 -l
    BOARD uno)
    