---
id: rVWqjtG6tA9UvKnP74NHn
title: Makefile
desc: ''
updated: 1639772405725
created: 1639772361844
---


### What is Makefile

File type that is used for compiling and linking programs from source code files. Makefiles contain five kinds of things: explicit rules, implicit rules, variable definitions, directives, and comments.

### Useful Makefile

This make file can be usefull for small projects

```shell

CC=gcc
RM=rm
CFLAGS=-g -Wall
OBJS=somefile.o
BIN=main

all:$(BIN)

main:$(OBJS)
    $(CC) $(CFLAGS) $(OBJS) -o main

%.o: %.c
    $(CC) $(CFLAGS) -c $< -o $@

clean: 
    $(RM) -r main *.o

```
