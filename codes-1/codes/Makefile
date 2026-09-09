CC = gcc
CFLAGS = -Wall -Wextra

program: main.o isOdd.o isEven.o
	$(CC) $(CFLAGS) -o program main.o isOdd.o isEven.o

main.o: main.c isEven.h isOdd.h
	$(CC) $(CFLAGS) -c main.c

isOdd.o: isOdd.c isOdd.h
	$(CC) $(CFLAGS) -c isOdd.c

isEven.o: isEven.c isEven.h
	$(CC) $(CFLAGS) -c isEven.c

clean:
	rm -f program *.o