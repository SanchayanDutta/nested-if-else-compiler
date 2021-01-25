# nested-if-else-compiler

lex lexer.l

yacc -d -v parser.y

gcc y.tab.c -ll

./a.out < input.txt

# Output

#######################################################################################
			Intermediate code
#######################################################################################
= 	 5	 x 
= 	 0	 y 
if x > 2 goto L0 else goto L20

 Label	L0:
= 	 1	 y 
goto next

Label	L20:
= 	 2	 y 
goto next

Label next:


-----------------------------------------------------------------------------------

			Syntax Tree in Inorder traversal
-----------------------------------------------------------------------------------
 start ,  definition ,  statement ,  definition ,  statement ,  x ,  = ,  5 ,  statement ,  y ,  = ,  0 ,  statement ,  x ,  > ,  2 ,  IF ,  y ,  = ,  1 , 



_______________________________________________________________________________________
Optimized  code
_______________________________________________________________________________________
=	0		x
=	0		y
=	0		y
=	0		y

Parsing is Successful


#######################################################################################
			Symbol table
#######################################################################################

symbol 	 type  	 identify 	 line number
_______________________________________________________________________________________
#include<stdio.h>		Header	0	
#include<stdlib.h>		Header	1	
int	N/A	KEYWORD		3	
main	int	IDENTIFIER	3	
(	N/A	Punctuation	3	
argv	int	IDENTIFIER	3	
,	N/A	Punctuation	3	
char	N/A	KEYWORD		3	
argc	char*	IDENTIFIER	3	
]	N/A	Punctuation	3	
)	N/A	Punctuation	3	
{	N/A	Punctuation	4	
;	N/A	Punctuation	5	
x	int	variable	5	
y	int	variable	6	
=	N/A	Operator	7	
5	int	NUMBER		7	
0	int	NUMBER		8	
if	N/A	KEYWORD		9	
>	int	IDENTIFIER	9	
2	int	NUMBER		9	
else	N/A	KEYWORD		13	
}	N/A	Punctuation	17	
}	N/A	punctuation	16
