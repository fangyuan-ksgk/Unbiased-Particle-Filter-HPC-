# Parallel-Particle-Filter(HPC)

This folder includes the Code to implement the Paralle Particle Filter (PPF, also known as the Unbiased Particle Filter) algorithm, as well as the Multilevel Particle Filte (MLPF), with example models upon which comparision between the two algorithms are provided. 

To demostrate the parallel power of PPF, a HPC implementation of PPF is also provided. Where we can see that the embarrasinly parallel structure of PPF, with no requirement of intercommunication by for the final collection, demostrate a linear speed-up with respect to the number of cores we have access to.

The file 'Parallel Particle Filter' contains code for PPF, as well as MLPF, tuning functions are also provided for their best performance on any partially observed diffusion with discrete observations models. A experiment section demonstrates the way we conduct numerical experiemnts to compare the performance of the two algorithms on a single processor.

The file 'HPC-PFF' provides HPC implementation of the PPF algorithms, the file is designed to run on KAUST supercomputer Shaheen.

The two .npy files store the observation as well as the fitted constants for the model where the signal process is a Ornstein-Uhlenbeck process.
