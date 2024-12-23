# JKFLIPFLOP-USING-IF-ELSE

**AIM:** 

To implement  JK flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**JK Flip-Flop**

JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/JKFLIPFLOP-USING-IF-ELSE/assets/154305477/a649c30b-232b-4558-b188-fd6c09845180)


This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs. The following table shows the state table of JK flip-flop.

![image](https://github.com/naavaneetha/JKFLIPFLOP-USING-IF-ELSE/assets/154305477/c4360742-e8a8-4937-b089-c46c0433f9a3)

 
Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop. Present Inputs Present State Next State
 
![image](https://github.com/naavaneetha/JKFLIPFLOP-USING-IF-ELSE/assets/154305477/6c275261-a6d5-4c37-a3a7-1e88ca11c4cd)

By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.
 
![image](https://github.com/naavaneetha/JKFLIPFLOP-USING-IF-ELSE/assets/154305477/5174f41b-0ce0-4329-a372-6d1943ea6673)

The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)

**TRUTH TABLE**

![Screenshot 2024-12-23 091744](https://github.com/user-attachments/assets/cbea7f8c-03a4-48ba-9d61-8cd106e36a5e)


**Procedure**

/*1.Type the program in Quartus software using Verilog.

 2.Compile and run the program.
 
 3.Generate the RTL schematic and save the logic diagram.
 
 4.Create nodes for inputs and outputs to generate the timing diagram.
 
 5.Generate the timing diagram for different input combinations. */

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming.
Developed by:R.karthik padmanaban
RegisterNumber:24001743
```
 module sr_ff(s,r,clk,q,qbar);
 input s,r,clk;
 output reg q;
 output reg qbar; initial
 begin
 q=0;
 qbar=1;
 end
 always @(posedge clk)
 begin
 q=s|(~r&q);
 qbar=r|(~s&~q);
 end
 endmodule
*/
```

**RTL LOGIC FOR FLIPFLOPS**

![Screenshot 2024-12-23 091944](https://github.com/user-attachments/assets/d28e2eac-8ddf-4590-91b6-ceafaa3bdf8c)


**TIMING DIGRAMS FOR FLIP FLOPS**

![Screenshot 2024-12-23 092019](https://github.com/user-attachments/assets/78521093-66b4-42d4-9355-2c3d71fc4dfa)


**RESULTS**
Thus the JK flipflop using verilog and validating their functionality using
their functional tables are verified
