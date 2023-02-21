calculator: main.o addition.o subtraction.o multiplication.o division.o operations.h
	cc main.o addition.o subtraction.o multiplication.o division.o -o calculator

main.o: main.c operations.h
	cc -c main.c

subtraction.o: subtraction.c operations.h
	cc -c subtraction.c

addition.o: addition.c operations.h
	cc -c addition.c

multiplication.o: multiplication.c operations.h
	cc -c multiplication.c

division.o: division.c operations.h
	cc -c division.c

objects = addition.o subtraction.o multiplication.o division.o main.o

clean:
	rm -f $(objects)

.PHONY: all

#main: $(objects)
#	cc -o main $(objects)
#

#$(objects): %.o:%.c operations.
#	cc -c $< -o $@
