To Run OpenMP Program: 

'''sh
g++ -o nbody_omp -fopenmp nbody_omp.C
time ./nbody_omp -t 10 < sample_input.in > omp_10.out
time ./nbody_omp -t 1000 < sample_input.in > omp_1000.out
time ./nbody_omp -t 1000000 < sample_input.in > omp_1000000.out
'''


On server: 

10: 
0.111u 0.006s 0:00.01 1100.0%    0+0k 8+8io 0pf+0w (with pragma)
0.082u 0.000s 0:00.01 800.0%    0+0k 0+8io 0pf+0w (wo pragma)
1000: 
1.475u 0.028s 0:00.11 1354.5%    0+0k 0+504io 0pf+0w (with pragma)
1.945u 0.055s 0:00.14 1421.4%    0+0k 0+512io 0pf+0w (wo pragma)
1000000: 
61.577u 15.083s 0:31.99 239.6%    0+0k 0+492552io 0pf+0w (with pragma)
60.169u 16.082s 1:45.65 72.1%    0+0k 0+499544io 0pf+0w (wo pragma)
