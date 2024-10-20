main:./lib/libcal.a
	gcc ./src/add.c ./src/sub.c main.c -o main -l cal -L ./lib -I ./include
./lib/libcal.a:
	gcc -c ./src/add.c -o ./src/add.o -I ./include
	gcc -c ./src/sub.c -o ./src/sub.o -I ./include	
	ar rcs libcal.a ./src/add.o ./src/sub.o
	mv libcal.a ./lib
.PHONY:clean
clean:
	rm ./src/add.o;
	rm ./src/sub.o
	rm ./main

