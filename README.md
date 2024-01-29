combinational corcuits Multiplexer. D multiplezer
ulkste Verilog code
Verify the Functionality using Test -berch.
cede:-
module mux_ 4 to 1 C
input wire [3:0] data-in,
input wire (1:0] sel,
output wire data -out
assign data-out = (Sel == 2'600)? data-in(0]:
(ser== 2'001)? data -in (i]:
(Se1 == 2'b01)? data - in (2]:
data -90(30:
end module
module tb-mux - 4 to1;
reg (3:01 data in:
reg [1:0] sel;
wire data -out;
mux_ 4t01 unt C
. data-in (data-in),
• sel (sel),
• data -out (data-out)
~
module demux-1104 C
Input wire d, input wire se output reg q0,
output reg q'; output reg 92, outputreg 93
always @ (posedges or poselged)
casels)
2'600: begin
q1 < = 1'60:
92 <= 1'b0;
93 <= 150:
end
2' bol i begin go L= 1'50 q' L=d:
92 25 160,
93 < 1'60: end
2' boo 1 begin
904=1b02
q1<= 1'60;
921=d:
93< =150: end
2'bll: begin
q1 < = 1'60;
922= 160;
93<= d;. end
default: begin q0<= 1'bo;
qi L= 1b0:
q21= 1'b0'
93<= 1'b0';
end endcase
end module anitial begin
data fn = 4'b|100;
sel = 2'500:
#10）
data in = 4'611001
sel = 2'011
#10
$finish:
end endmodule.
