# AIM: 

To simulate and synthesis of JK_flipflop using vivado 2023.2

# APPARATUS REQUIRED:

vivado 2023

# PROCEDURE:

STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button.

Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.

# JK_FLIPFLOP
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/094e9d55-5f30-4984-90b9-dd51d5297974)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/5b973ee8-9ee2-402d-8cba-1adfa2e4d5f2)
# Truth Table
![image](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/154305926/04d4ff52-ae20-4e08-bd70-58137b129890)
# verilog code
```
module jk(j,k,clk,rst,Q);
input j,k,clk,rst;
output reg Q;
always @(posedge clk)
begin
if(rst==1)
Q=0;
else
begin
case({j,k})
2'b00:Q=Q;
2'b01:Q=0;
2'b10:Q=1;
2'b11:Q=~Q;
endcase
end
end
endmodule
```
# output
![318284015-3365ac51-9f03-4a25-ab85-97981165b9c2](https://github.com/RESMIRNAIR/JK_FLIPFLOP/assets/160302888/2cbd5ca5-0d5e-42c3-aaab-11a60ef61971)
# Result

Thus the simulation and synthesis of JK_flipflop using vivado 2023.2 is successfully executed and verified.
