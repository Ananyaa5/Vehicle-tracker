# Vehicle-tracker
The project consists of the code required for a vehicle tracker. Hardware used - Arduino uno, Ublox neo 6m GPS module, SIM900A GSM module

Connections:
GPS module - TX- D4 on arduino
             RX- D3 on arduino
GSM module - 5TX - D0 on arduino
             5RX - D1 on arduino

Connect Vcc and GND of both the modules to 5V and GND pins of arduino respectively

The coordinates will be sent when a message "TRACK" has been sent to the SIM present inside the SIM900A module. On receiving this message, the arduino will send a reply message consisting of the coordinates to the mobile number given in the code through the GSM module.
The reply would take about 20 seconds to be received.
