To Run Sequential Program: 
'''sh
g++ -o nbody_seq nbody_seq.C
time ./nbody_seq -t 10 < sample_input.in > seq_10.out
time ./nbody_seq -t 1000 < sample_input.in > seq_1000.out
time ./nbody_seq -t 1000000 < sample_input.in > seq_1000000.out
'''

On Local: 
./nbody_seq -t 10 < figure8.in > seq_10.out  0.00s user 0.00s system 66% cpu 0.009 total

./nbody_seq -t 1000 < figure8.in > seq_1000.out  0.07s user 0.04s system 94% cpu 0.112 total

./nbody_seq -t 1000000 < figure8.in > seq_1000000.out  65.83s user 26.75s system 99% cpu 1:33.14 total




On server: 
10:
0.001u 0.000s 0:00.00 0.0%    0+0k 64+8io 2pf+0w
1000: 
0.045u 0.020s 0:00.09 66.6%    0+0k 0+528io 0pf+0w
1000000: 
47.734u 14.316s 1:08.16 91.0%    0+0k 0+527360io 0pf+0w
