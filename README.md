# nested-if-else-compiler

Use the following commands to run the program. This will require installation of **Lex** and **Yacc**.

lex lexer.l

yacc -d -v parser.y

gcc y.tab.c -ll

./a.out < input.txt
