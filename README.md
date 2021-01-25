# if-else-compiler

To run program:

lex lexer.l
yacc -d -v parser.y
gcc y.tab.c -ll
./a.out < input.txt
