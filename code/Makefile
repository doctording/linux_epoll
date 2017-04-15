.PHONY: build clean

CC=g++
HEADERS=-I.
DEBUG=-g -ggdb  
WALL=-Wall -W  
CFLAGS=$(WALL) $(DEBUG)  
L_CC=$(CC) $(CFLAGS) $(HEADERS)     

build:server client

server:server.cpp
	$(L_CC) $< -o $@

client:client.cpp
	$(L_CC) $< -o $@

clean:
	@-if [ -f server ]; then rm server; fi
	@-if [ -f client ]; then rm client; fi
	@rm -rf *~
