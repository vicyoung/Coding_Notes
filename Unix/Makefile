# Makefile variables
CC=g++
CFLAGS=-g -Wall
LDFLAGS=
RM=rm -rf

# Sources, headers, objects, and executable
SRCS=$(wildcard *.cc)
HDRS=$(wildcard *.h)
OBJS=$(SRCS:.cc=.o)
EXEC=main

# Executable
default: $(EXEC)

# Linker
$(EXEC): $(OBJS)
        $(CC) $(LDFLAGS) -o $@ $(OBJS)

# Compiler
.cc.o: $(SRCS) $(HDRS)
        $(CC) $(CFLAGS) -o $@ -c $<
