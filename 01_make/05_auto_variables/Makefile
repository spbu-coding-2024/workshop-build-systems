TARGET = hello

CC = gcc
CFLAGS = -O2

.PHONY: all clean

all: $(TARGET)

main.o: main.c
	$(CC) $(CFLAGS) -c $< -o $@

hello.o: hello.c
	$(CC) $(CFLAGS) -c $< -o $@

$(TARGET): main.o hello.o
	$(CC) $(LDFLAGS) $^ -o $@

clean:
	$(RM) $(TARGET) *.o
