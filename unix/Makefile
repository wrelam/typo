# BSD make syntax
APP 	= typo
C_SRC 	!= ls *.c
OBJS 	= $(C_SRC:.c=.o)

.SUFFIXES: .c

.PHONY: all
all: ${OBJS}
	$(CC) $(CFLAGS) -o $(APP) ${OBJS}

.c.o:
	$(CC) $(CFLAGS) -c ${.IMPSRC}

.PHONY: clean
clean:
	rm -f $(APP) *.o

