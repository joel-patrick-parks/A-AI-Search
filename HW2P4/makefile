CC = g++
CFLAGS = -O0

default: hw2

hw2: Main.o
	$(CC) -std=c++0x $(CFLAGS) -o hw2 Main.o

Main.o: Main.cpp
	$(CC) -std=c++0x $(CFLAGS) -c Main.cpp

clean:
	$(RM) count *.o *~