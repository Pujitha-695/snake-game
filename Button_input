`timescale 1ns / 1ps

module button_input( l,r,u,d,clk,direction );
input l,r,u,d,clk;
output reg [3:0]direction;

always@(posedge clk)
begin
if(l == 1) begin direction <= 4'b0001; end //left
else if(r == 1) begin direction <= 4'b0010; end //right
else if(u == 1) begin direction <= 4'b0100; end //up
else if(d == 1) begin direction <= 4'b1000; end //down
else begin direction <= direction; end //no change in direction
end

endmodule
