# Parallelization:  Sieve of Eratosthenes
# By Aaron Weeden, Shodor Education Foundation, Inc.
# January 2012
#
# Makefile
#
# Usage:  On the command line, enter 'make' followed by one of the options below
# e.g. $ make serial

serial:
	gcc -o sieve.serial sieve.serial.c -lm
openmp:
	gcc -fopenmp -o sieve.openmp sieve.openmp.c -lm
mpi:
	mpicc -o sieve.mpi sieve.mpi.c -lm
hybrid:
	mpicc -fopenmp -o sieve.hybrid sieve.hybrid.c -lm
all:
	make clean
	make serial openmp mpi hybrid
clean:
	rm -rf sieve.{serial,openmp,mpi,hybrid}
