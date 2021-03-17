Problem 4.7 from the text.

In addition, as we did in class, implement these MIPS instructions on the single cycle datapath:

1. blt instruction - I type instruction that has the following effect:

if (R[rs] < R[rt])

PC = PC + 4 + SE(I)

else

PC = PC + 4

2. jal instruction - J type instruction that has the following effect:

R[$r31] = PC+4

PC = [31..28](PC+4) | [27..0] (I<<2)

(in other words, this works exactly like the jump instruction we covered but also writes PC+4 to register $r31 - and always writes to register $r31)

3. jr instruction - R type instruction that has the following effect:

PC = R[rs]
