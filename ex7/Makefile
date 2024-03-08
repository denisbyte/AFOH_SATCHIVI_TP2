# Compiler options
CC = gcc
CFLAGS = -Wall -Wextra -std=c99 -g

# Source files
SRC = lock.c

# Object files
OBJ = $(SRC:.c=.o)

# Executable name
EXEC = prog

# Rule to compile .c files into .o files
%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# Rule to build the executable
$(EXEC): $(OBJ)
	$(CC) $(CFLAGS) $(OBJ) -o $(EXEC)

# Clean rule
clean:
	rm -f $(OBJ) $(EXEC)

# Phony target to avoid conflicts with file names
.PHONY: clean