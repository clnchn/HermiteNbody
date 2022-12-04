To Run Sequential Program: 
'''sh
g++ -o nbody_seq nbody_seq.C
time ./nbody_seq -t 10 < figure8.in > seq_10.out

time ./nbody_seq -t 100000 < figure8.in > seq_100000.out

time ./nbody_seq -t 1000000 < figure8.in > seq_1000000.out
'''

./nbody_seq -t 10 < figure8.in > seq_10.out  0.00s user 0.00s system 66% cpu 0.009 total

./nbody_seq -t 1000 < figure8.in > seq_1000.out  0.07s user 0.04s system 94% cpu 0.112 total

./nbody_seq -t 1000000 < figure8.in > seq_1000000.out  65.83s user 26.75s system 99% cpu 1:33.14 total


0.001u 0.000s 0:00.00 0.0%    0+0k 32+0io 0pf+0w

10000:

