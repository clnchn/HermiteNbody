To Run OpenMP Program: 

'''sh
g++ -o nbody_omp nbody_omp.C
time ./nbody_omp -t 10 < sample_input.in > omp_10.out

time ./nbody_omp -t 1000000 < sample_input.in > omp_1000000.out
'''
