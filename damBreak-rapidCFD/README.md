cells:            5670000

GeForce GTX 980M
- at Time = 0.0902955: deltaT = 0.000121065 sec, ExecutionTime = 54235.6 s  ClockTime = 54289 s
- Clock time at end of previous time: ExecutionTime = 54143.2 s  ClockTime = 54197 s
- Clocktime for one step = 92 seconds

- at Time = 0.402058: delta T = 0.000121065 sec, ExecutionTime = 332261 s  ClockTime = 332437 s
- Clock time at end of previous time: ExecutionTime = 332195 s  ClockTime = 332370 s
- Clocktime for one step = 67 seconds

Intel(R) Core(TM) i7-5960X CPU @ 3.00GHz
- OpenFOAM 5.0-dbb428a3a855
- Single core calculation
- At Time = 0.0902975, deltaT = 1.62794e-05 sec, ExecutionTime = 398585 s  ClockTime = 398600 s
- Clock time at end of previous time: ExecutionTime = 398308 s  ClockTime = 398322 s
- Clocktime for one step = 278 seconds

Analysis
At same time (0.0902955 sec), Rapid CFD = 7.34x CPU net overall speed up at 0.092955 sec.

However, the RapidCFD calculation appears to be speeding up. Considering both deltaT and elapsed time at 
a given time step, RapidCFD is running ~22x faster than OpenFOAM at the 0.0902955 sec time step:
- RapidCFD: 0.000121065 sec / 92 sec = 1.31E-6 sec/sec
- CPU: 1.62794e-05 sec / 278 sec = 5.85E-8 sec/sec

At 0.402058sec, RapidCFD is running ~30x faster than OpenFOAM at 0.0902975sec:

- RapidCFD: 0.000121065 sec / 67 sec = 1.81E-6 sec/sec
- CPU: 1.62794e-05 sec / 278 sec = 5.85E-8 sec/sec


Important note: This case requires > 5 GB RAM and will not run on a single K20 GPU

