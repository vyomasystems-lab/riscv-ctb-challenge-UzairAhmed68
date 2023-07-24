After running make, error results in lines 15855 and 25584 with errors: Error: illegal operands `and s7,ra,z4' 
and Error: illegal operands `andi s5,t1,s0' respectively.

For the line `and s7,ra,z4', there is no variable decleared as z4 hence correcting
z4 to s4 will absolve the error

For the line `andi s5,t1,s0', the instruction demands an immediate value  rather than
a register value hence correcting s0 to 0 will absolve the error

correcting these 2 errors will let the make file run properly 

