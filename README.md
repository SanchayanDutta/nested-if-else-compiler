# nested-if-else-compiler

lex lexer.l

yacc -d -v parser.y

gcc y.tab.c -ll

./a.out < input.txt
