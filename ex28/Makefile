CFLAGS = -Wall -Wextra
CC = gcc

.PHONY: all clean

all: calculator

calculator: main.o math.utils.o
	$(CC) $(CFLAGS) $^ -o $@

main.o: main.c math_utils.h
	$(CC) $(CFLAGS) -c $< -o $@

math_utils.o: math_utils.c math_utils.h
	$(CC) $(CFLAGS) -c $< -o $@
clean:
	rm -f calculator main.o math_utils.o
