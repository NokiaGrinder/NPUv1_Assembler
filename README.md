https://docs.google.com/spreadsheets/d/1OF3O5bw2V21qnUeJBV3uVHw2QGQBGvBB6mRa1SmMSnI/edit?gid=0#gid=0
NPUv1 ISA (Instruction Set Architecture) (RISC)

How code is to be structured:

Note: All instructions are to be written like their ISA counterparts. The name of the instruction is their Mneumonics in the ISA.

.exm add r1 r2 r3
     xor r1 r2 r3
     rsh r1 r2
     jmp .exm
     nop
     hlt

For Branching check the notes tabs on Flags and Cond for more info about what the first number does.

.col brh 1 45
     brh 2 .col

before each line of code, 5 spaces are to be made. Ex:

     add r1 r2 r3

if labels. Ex:

.exm add r1 r2 r3

For Loops. Labels cannot be added to for loops:

     Forl n rx ry
     -nop
     -add r1 r2 r3

n = number of times you want to loop for. (1->n)
rx = register that stores current count value
ry = register that stores n
