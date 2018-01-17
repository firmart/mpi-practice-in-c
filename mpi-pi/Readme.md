The program `mpi-pi` compute pi value using the following identity :

![](https://latex.codecogs.com/gif.latex?%5Cint_0%5E1%5Cfrac%7B4%7D%7B1&plus;x%5E2%7D%5C%2C%5Cmathrm%7Bd%7Dx%20%3D%20%5Cpi)

# MPI Routine

The following MPI routine are used :

* `int MPI_Init(int * argc, char *** argv)`
* `int MPI_Comm_size(MPI Comm comm, int * size)`
* `int MPI_Comm_rank(MPI Comm comm, int * rank)`
* `int MPI_Bcast(void * buf, int count, MPI Datatype datatype, int root, MPI Comm comm)`
* `int MPI_Reduce(const void * sendbuf, void * recvbuf, int count, MPI Datatype datatype, MPI Op op, int root, MPI Comm comm)`
* `int MPI_Finalize()`

# Compilation & Execution

Compilation :
`mpicc mpi-pi.c -o mpi-pi`
Execution :
`mpirun -np 2 mpi-pi`

# Reference 

* Using MPI, 3rd ed.