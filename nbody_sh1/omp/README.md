To Run OpenMP Program: 

'''sh
g++ -o nbody_omp -fopenmp nbody_omp.C
time ./nbody_omp -t 10 < sample_input.in > omp_10.out
time ./nbody_omp -t 1000 < sample_input.in > omp_1000.out
time ./nbody_omp -t 1000000 < sample_input.in > omp_1000000.out
'''


./nbody_omp -t 10 < sample_input.in > omp_10.out  0.00s user 0.01s system 65% cpu 0.013 total

./nbody_omp -t 1000 < sample_input.in > omp_1000.out  0.07s user 0.03s system 96% cpu 0.104 total

./nbody_omp -t 1000000 < sample_input.in > omp_1000000.out  65.75s user 24.79s system 99% cpu 1:31.21 total



0.156u 0.003s 0:00.02 750.0%    0+0k 0+8io 0pf+0w
1000:
10.805u 0.136s 0:00.70 1561.4%    0+0k 0+528io 0pf+0w
8.561u 0.120s 0:00.56 1550.0%    0+0k 0+528io 0pf+0w
72.461u 25.739s 0:11.05 888.5%    0+0k 0+528io 0pf+0w

10000:
88.789u 0.998s 0:07.88 1139.2%    0+0k 0+5280io 0pf+0w

100000:
934.380u 9.793s 1:27.65 1077.2%    0+0k 0+52768io 0pf+0w

1000000: 
5267.257u 51.230s 7:05.26 1250.6%    0+0k 0+229064io 0pf+0w
