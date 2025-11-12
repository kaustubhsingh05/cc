# cc

for only .l

gedit prac.l
lex prac.l
gcc lex.yy.c -o prac -lfl
./prac

for both
gedit prac.l
gedit prac.y

yacc -d prac.y
lex prac.l
gcc lex.yy.c y.tab.c -o icgen -ll
./icgen
