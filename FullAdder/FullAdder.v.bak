module fulladder4(A,B,Cin,SUM,Cout);
output[3:0] SUM;
output Cout;
input[3:0] A,B;
input Cin;
assign{Cout,SUM} = A+B+Cin;
endmodule
///////////

module TB_FA();
	reg[3:0]a,b;
        reg c_in;
        wire[3:0]s;
        wire c_o;
        fulladder4 f1(.A(a),.B(b),.Cin(c_in),.SUM(s),.Cout(c_o));
initial
	begin
		a=4'b0000;b=4'b0001;c_in=1'b0;
		#100;
                a=4'b0011;b=4'b0011;c_in=1'b0;
		#100;
		a=4'b0111;b=4'b1011;c_in=1'b0;
		#100;
  		a=4'b0011;b=4'b0001;c_in=1'b0;
		#100;
	end
endmodule