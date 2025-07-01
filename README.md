
### Run
To build the executable:
```bash
$ cd FK
$ module load gcc-glibc dealii
$ ./test.sh
```
The executable will be created into `build`, and can be executed through
```bash
$ ./FK_solver
```
or 
```bash
mpirun --allow-run-as-root -np <number of cores> ./FK_solver
```
If you still run this in docker, try
```bash
mpirun --allow-run-as-root -np <number of cores> --mca btl tcp,self ./FK_solver
```
