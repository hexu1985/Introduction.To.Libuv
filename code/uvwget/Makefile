
RM = rm -f
CC = gcc
CFLAGS = -Wall -g 
INCLUDES = -I../../libuv/include
LDFLAGS = -luv_a -lcurl -lpthread -ldl
LDPATH = -L../../libuv/build

SOURCES = $(shell ls *.c)
PROGS = $(subst .c,,$(SOURCES))
#PROGS = $(SOURCES:%.c=%)

all: $(PROGS)
	@echo "PROGS = $(PROGS)" 

clean:
	$(RM) $(PROGS)

%: %.c
	$(CC) -o $@ $(CFLAGS) $(INCLUDES) $^ $(LDFLAGS) $(LDPATH)
