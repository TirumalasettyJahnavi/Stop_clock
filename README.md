# Stop_clock
Verilog Implementation of a Stopwatch on an FPGA

The core of this design is a counter that increments every second. The "start" and "stop" conditions are not simple edge detections but rather a long press of a button. This requires a separate timing mechanism to detect the 10-second button press.

**Button Press Duration**
To detect a 10-second press, you need a separate counter for each button.

**Start Button Logic**: When the debounced start_btn is pressed, a counter starts counting up to 10 seconds. If the button is held for the full 10 seconds, a start_condition signal becomes active. If the button is released before 10 seconds, the counter resets.

**Stop Button Logic**: Similarly, a separate counter for the stop_btn checks for a 10-second press, activating a stop_condition signal.

