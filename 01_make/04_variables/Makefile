TARGET = hello

CC = gcc
CFLAGS = -O2

.PHONY: all clean

all: $(TARGET)

main.o: main.c
	$(CC) $(CFLAGS) -c main.c -o main.o

hello.o: hello.c
	$(CC) $(CFLAGS) -c hello.c -o hello.o

$(TARGET): main.o hello.o
	$(CC) main.o hello.o -o $(TARGET)

clean:
	rm -rf $(TARGET) *.o
