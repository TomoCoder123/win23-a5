# Compiler
CC = gcc
CFLAGS = -Wall -std=c11 -g

SRCS = main.c addition.c subtraction.c multiplication.c division.c
OBJS = $(SRCS:.c=.o)

DEPS = operations.h

TARGET = calculator

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

%.o: %.c $(DEPS)
	$(CC) $(CFLAGS) -c $< -o $@

.PHONY: clean
clean:
	-del /F /Q $(TARGET) $(OBJECTS) 2>nul
