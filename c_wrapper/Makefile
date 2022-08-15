
# Define required macros here
SHELL = /bin/sh
PROJECT = Fred
OBJS =  MyClass.o MyWrapper.o MyMain_c.o  
CFLAG = -Wall -g
CC = gcc
CXX = g++
INCLUDE =
LIBS = 

all : ${PROJECT}
.PHONY : all 

${PROJECT}: ${OBJS}
	${CXX} ${CFLAGS} ${INCLUDES} -o $@ ${OBJS} ${LIBS}

%.o : %.cpp
	$(CXX) $(CXXFLAGS) -o $@ -c $<

%.o : %.c
	$(CC) $(CFLAGS) -o $@ -c $<

.PHONY: clean
clean:
	rm -f *.o core *.core



	