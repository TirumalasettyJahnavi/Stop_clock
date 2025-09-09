# Stop_clock
Verilog Implementation of a Stopwatch on an FPGA
I have implemented stop clock using verilog HDL in Xilinx VIVADO.Solved the errors and simulation result is obtained.
Synthesized the code and generated the bit stream file.Assigned the pins of FPGA on pin planner and dumped the code onto the board.

**Button Press Duration**
To detect a 10-second press, I need a separate counter for each button.

**Start Button Logic:** When the debounced start_btn is pressed, a counter starts counting up to 10 seconds. If the button is held for the full 10 seconds, a start_condition signal becomes active. If the button is released before 10 seconds, the counter resets.

**Stop Button Logic:** Similarly, a separate counter for the stop_btn checks for a 10-second press, activating a stop_condition signal.

On 10sec long press of start push button the clock is started and on 10sec long press of stop push button the clock is stopped.

THIS PROJECT IS CARRIED IN THE PROCESS OF TRAINING FROM THE SSIT PVT LIMITED.







