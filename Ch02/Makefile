# Author: Matthew Morrison
# E-mail: matt.morrison@nd.edu
#
# This is the Makefile for Chapter 2 - Into the Void

# G++ is for the GCC compiler for C++
PP := g++

# CFLAGS are the compiler flages for when we compile C code in this course
FLAGS := -O0 -g -Wall -Wextra -Wconversion -Wshadow -pedantic -Werror -lm
CXXFLAGS := -m64 -std=c++11 -Weffc++ $(FLAGS)



# Compilation for the "nothing" program
# Command: make nothing
nothingObjs :=  nothing.o

nothing: nothing.o
	$(PP) $(CXXFLAGS) -o nothing $(nothingObjs)

nothing.o: nothing.cpp
	$(PP) $(CXXFLAGS) -c nothing.cpp



# C++ Hello, World Example
# Command: make hello
helloObjs :=  hello.o

hello: hello.o
	$(PP) $(CXXFLAGS) -o hello $(helloObjs)

hello.o: hello.cpp
	$(PP) $(CXXFLAGS) -c hello.cpp



# Prints examples of ASCII char to terminal
# Command: make ascii
asciiObjects := ascii.o

ascii: $(asciiObjects)
	$(PP) $(CXXFLAGS) -o ascii $(asciiObjects)

ascii.o: ascii.cpp
	$(PP) $(CXXFLAGS) -c ascii.cpp


# Shows example of functions
# Command: make squareFunc
squareFuncObjects := squareFunc.o

squareFunc: $(squareFuncObjects)
	$(PP) $(CXXFLAGS) -o squareFunc $(squareFuncObjects)

squareFunc.o: squareFunc.cpp
	$(PP) $(CXXFLAGS) -c squareFunc.cpp


# Make all
all: nothing hello ascii squareFunc

# Make clean
clean :
	rm -rf *.o nothing hello ascii squareFunc
