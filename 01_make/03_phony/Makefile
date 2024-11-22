.PHONY: all
all: hello

hello: main.o hello.o
	gcc -o hello main.o hello.o

main.o: main.c
	gcc -c -o main.o main.c

hello.o: hello.c
	gcc -c -o hello.o hello.c

.PHONY: clean
clean:
	rm -rf hello *.o
