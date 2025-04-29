# dse-lab-5-fsm-solved
**TO GET THIS SOLUTION VISIT:** [DSE Lab#5-FSM Solved](https://www.ankitcodinghub.com/product/dse-solved-5/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;113235&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;DSE Lab#5-FSM  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
&nbsp;

This lab aims at investigating the operation of Finite State Machines. You will need to implement different FSM by starting from different design hypotheses. Hence, you will learn how to design an FSM by using the VHDL description language. For each of the following designs you have to provide a hand-written block scheme of what you will describe in VHDL.

Contents:

1. One-Hot Finite state machine

2. Modified One-Hot FSM

2. Two-process FSM

3. “HELLO” FSM

Abbreviations and acronyms: FSM – Finite State Machine

IC – Integrated Circuit

LED – Light Emitting Diode

MUX – Multiplexer

RTL – Register Transfer Level

VHDL – Very high speed integrated circuits Hardware Description Language

1 – One-Hot Finite state machine

We want to implement a Finite State Machine (FSM) that recognizes two specific sequences of input symbols, namely four consecutive 1s or four consecutive 0s. Summarizing we have an input w and the FSM gives an output z. Whenever w = 1 or w = 0 for four consecutive clock pulses the value of z has to be 1; otherwise, z = 0. Overlapping sequences are allowed, so that if w = 1 for five consecutive clock pulses the output z will be equal to 1 after the fourth and fifth pulses. Figure 1 illustrates the required relationship between w and z.

Figure 1 – Required timing for the output z.

A state diagram for this FSM is shown in Figure 2. For this part you need to manually derive an FSM circuit that implements this state diagram, including the logic expressions that feed each of the state flip-flops. To implement the FSM use nine state flip-flops called y8, . . . , y0 and the one-hot state assignment given in Table 1.

Table 1 – One-hot codes of the FSM.

Design and implement your circuit on the DE1 board as follows:

1. Create a new Quartus Prime project for the FSM circuit. Select as the target chip the Cyclone V 5CSEMA5F31C6, which is the FPGA chip on the Altera DE1 board.

2. Write a VHDL file that instantiates the 9 flip-flops and specifies the logic expressions that drive the flip-flop input ports. Use only simple assignment statements in your VHDL code to specify the logic feeding the flip-flops. Note that the one-hot code enables you to derive these expressions by inspection. Use the toggle switch SW0 on the Altera DE1 board as an active-low synchronous reset input for the FSM, use SW1 as the w input, and the push button KEY0 as the clock input which is applied manually. Use the red LED LEDR0 as the output z.

3. Include the VHDL file in your project, and assign the pins on the FPGA to connect to the switches and the LEDs, as indicated in the User Manual for the DE1 board. Compile the circuit.

4. Simulate the behavior of your circuit.

5. Once you are confident that the circuit works properly as a result of your simulation, download the circuit into the FPGA chip. Test the functionality of your design by applying the input sequences and observing the output LEDs. Make sure that the FSM properly generates the correct output values on LEDR0.

Figure 2 – A state diagram of the FSM.

2 – Modified One-Hot FSM

Consider a modification of the one-hot code given in Table 1. When an FSM is going to be implemented in an FPGA, the circuit can often be simplified if all flip-flop outputs are 0 when the FSM is in the reset state. This approach is preferable because the FPGA’s flip-flops usually include a clear input port, which can be conveniently used to realize the reset state, but the flip-flops often do not include a set input port.

Table 2 shows a modified one-hot state assignment in which the reset state, A, uses all 0s. This is accomplished by inverting the state variable y0. Create a modified version of your VHDL code that implements this state assignment. Hint: you should need to make very few changes to the logic expressions in your circuit to implement the modified codes. Compile your new circuit and test it both through simulation and by downloading it onto the DE1 board. Keep the same pin assignment.

3 – Two-process FSM

For this part you need to write another style of VHDL code for the FSM in Figure 2. In this version you should not manually derive the logic expressions needed for each state flip-flop. Instead, describe the state table for the FSM by using a VHDL CASE statement in a PROCESS block, and use another PROCESS block to instantiate the state flip-flops. You can use a third PROCESS block or simple assignment statements to specify the output z.

A VHDL code template is given in Figure 3. Observe that the present and next state vectors of the FSM are defined as an enumerated type with possible values given by the symbols A to I. The VHDL compiler determines how many state flipflops the circuit requires and it automatically chooses the state assignment.

Table 2 – Modified one-hot codes of the FSM.

LIBRARY ieee;

USE ieee.std_logic_1164.all;

ENTITY part2 IS

PORT ( . . . define input and output ports

. . .);

END part2;

ARCHITECTURE Behavior OF part2 IS

. . . declare signals

TYPE State_type IS (A, B, C, D, E, F, G, H, I);

SIGNAL y_Q, Y_D : State_type; — y_Q is present state, y_D is next state BEGIN

. . .

PROCESS (w, y_Q) — state table

BEGIN

CASE y_Q IS

WHEN A =&gt; IF (w = ‘0’) THEN Y_D &lt;= B;

ELSE Y_D &lt;= F;

END IF;

. . . other states

END CASE;

END PROCESS; — state table

PROCESS (Clock) — state flip-flops

BEGIN

. . .

END PROCESS;

. . . assignments for output z and the LEDs

END Behavior;

Figure 3 – VHDL code template of the FSM.

Implement your circuit as follows:

1. Create a new project for the FSM. Select as the target chip the Cyclone V 5CSEMA5F31C6N.

2. Include in the project your VHDL file that has the style of code in Figure 3. Use the toggle switch SW 0 on the Altera DE1 board as an active-low synchronous reset input for the FSM, use SW1 as the w input, and the pushbutton KEY0 as the clock input which is applied manually. Use the red LED LEDR0 as the output z. Assign the pins on the FPGA to connect to the switches and the LED, as indicated in the User Manual for the DE1 board.

3. Before compiling your code it is possible to tell the Synthesis tool in Quartus Prime what style of state assignment it should use. Choose Assignments &gt; Settings in Quartus Prime, and then click on the Compiler Settings item on the left side of the window. Then click on Advanced Settings (Synthesis)… then look for State Machine Processing and set Minimal Bits, as indicated in Figure 4.

4. To examine the circuit produced by Quartus Prime open the RTL Viewer tool. Double-click on the box shown in the circuit that represents the finite state machine, and determine whether the state diagram that it shows properly corresponds to the one in Figure 2.

5. Simulate your circuit.

6. Once you are confident that the circuit works properly as a result of your simulation, download the circuit into the FPGA chip. Test the functionality of your design by applying the input sequences and observing the output LEDs.

7. In step 3 you instructed the Quartus Prime Synthesis tool to use the state assignment given in your VHDL code. To see the result of changing this setting, open again the Quartus Prime settings window by choosing Assignments &gt; Settings, and click on the Compiler Settings item. Change the setting for State Machine Processing from Minimal Bits to One-Hot. Recompile the circuit and then open the report file, select the Analysis and Synthesis section of the report, and click on State Machines. Compare the state codes shown to those given in Table 2, and discuss any differences that you observe.

(a) – Settings Window

(b) – State Machine Processing ComboBox

Figure 4 – Specifying the state assignment method in Quartus Prime.

4 – “HELLO” FSM

Here you need to design a circuit for the DE1 board that scrolls the word “HELLO” in ticker-tape fashion on the six 7-segment displays HEX5 − 0. The letters should move from right to left in intervals of about one second. After the word “HELLO” scrolls off the left side of the displays, it should then start again on the right side.

Design your circuit by using six 7-bit registers connected in a queue-like fashion, in such a way that the outputs of the first register feed the inputs of the second one, the second feeds the third one, and so on (pipeline). Each register’s outputs should directly drive the seven segments of one display.

You need to design a finite state machine that controls the pipeline in two ways:

1. For the first six seconds after the system has been reset, the FSM inserts the correct characters (H,E,L,L,O, ) into the first of the 7-bit registers in the pipeline.

2. After step 1 is complete, the FSM configures the pipeline into a loop that connects the last register back to the first one, so that the letters continue to scroll indefinitely every second. Your circuit should scroll the word “HELLO” such that the letters move from right to left. Scrolling should continue indefinitely; after the word “HELLO” scrolls off the left side of the displays it should start again on the right side.

3. Write your VHDL code for the ticker-tape circuit and create a Quartus Prime project for your design. Use the 50MHz clock signal, CLOCK_50, on the DE1 board to clock the FSM and pipeline registers and use KEY0 as a synchronous active-low reset input. Write VHDL code in the style shown in Figure 3 for your finite state machine, and ensure that all flip-flops in your circuit are clocked directly by the CLOCK_50 input. Do not derive or use any other clock signals in your circuit.

4. Compile your VHDL code, download it onto the DE1 board and test the circuit.
