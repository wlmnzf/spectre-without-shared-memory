FILES=$(wildcard *.c)
TARGETS=$(FILES:.c=)
OBJS=${FILES:.c=.o}
CFLAGS=-g -std=gnu99 -I../src
# LDFLAGS=-L../src/ -g
LDLIBS=-lpthread


all: ${TARGETS}

${TARGETS}: %: %.o 
	${CC}  -o $@ $@.o ${LDLIBS}


clean:
	rm -f ${TARGETS} ${OBJS} *.sig out


