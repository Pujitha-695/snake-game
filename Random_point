`timescale 1ns / 1ps

module random_point( VGA_clk , rand_x, rand_y );
input VGA_clk;
output reg [9:0]rand_x;
output reg [9:0]rand_y;

reg [9:0] i = 0;
reg [9:0] j = 450;
always@(posedge VGA_clk)
begin
if( i < 610)
i <= i + 1'b1;
else
i <= 10'b0;
end

always@(posedge VGA_clk)
begin
if( j > 0)
j <= j - 1'b1;
else
j <= 10'd480;
end

always@(i,j)
begin
rand_x <= i;
rand_y <= j;
end
