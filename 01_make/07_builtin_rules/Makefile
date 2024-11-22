TARGET = hello

SOURCES = $(wildcard *.c)
OBJECTS = $(patsubst %.c,%.o,$(SOURCES))

.PHONY: all
all: $(TARGET)

$(TARGET): $(OBJECTS)

$(OBJECTS): %.o: %.c

.PHONY: clean
clean:
	$(RM) $(TARGET) $(OBJECTS)
