Problems 4.13.1, 4.14.1 (don't worry about delay slots - assume that branches resolve in the EX stage), 4.16.1-4.16.3

And - for the code sequence in 4.13, how many cycles would it take to execute this code on the 5-stage pipelined datapath with forwarding logic?

And - for the code sequence in 4.14, show the pipeline diagram (e.g. as we did in class) for the following cases:
a) full forwarding, branches resolved in EX

b) full forwarding, branches resolved in ID

For homework question 4.14, the branch pattern for "beq r2, r0, label2" is that it is not taken once and then taken. However, as written, neither r2 or r0 will change between executions of beq which means that the branch pattern cannot differ. As a result, "label1:" should be placed before the first instruction "lw r2, 0(r1)".
