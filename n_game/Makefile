# Makefile
.PHONY: all clean install uninstall

CC=gcc
CFLAGS=-C -Wall
SOURCES=src/game.c src/sys_utils.c
TARGET=bin/game
PREFIX_I=/usr/local/bin
PREEFIX_U=/usr/local

all: game

game:
	$(CC) $(CFLAGS) $(SOURCES) -o $(TARGET)

install:
	install $(TARGET) $(PREFIX)

clean: uninstall
	rm $(TARGET)

uninstall:
	rm $(PREFIX)/$(TARGET)
