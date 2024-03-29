# Unbiased Particle Filter (HPC)

This folder includes the Code to implement the Unbiased Particle Filter (UPF) algorithm, as well as the Multilevel Particle Filte (MLPF), with example models upon which comparision between the two algorithms are provided.

In the notebook, we also refer to UPF as the parallel particle filter, or PPF.

To demostrate the parallel power of UPF, a HPC implementation of UPF is also provided. Where we can see that the embarrasinly parallel structure of UPF, with no requirement of intercommunication by for the final collection, demostrate a linear speed-up with respect to the number of cores we have access to.

See our paper "Unbiased Filtering of a Class of Partially Observed Diffusions", first draft available on arXiv with the link: 
https://arxiv.org/abs/2002.03747

Many Thanks to my collaborators: Professor Ajay Jasra (KAUST), Professor Kody Law (Manchester).

@Fangyuan_ksgk

File-wise Description:

The file 'Unbiased Particle Filter' contains code for UPF, as well as MLPF, tuning functions are also provided for their best performance on any partially observed diffusion with discrete observations models. An experiment section demonstrates the way we conduct numerical experiemnts to compare the performance of the two algorithms on a single processor.

The file 'HPC-UPF' provides HPC implementation of the UPF algorithms, the file is designed to run on KAUST supercomputer Shaheen.

The two .npy files store the observation as well as the fitted constants for the model where the signal process is a Ornstein-Uhlenbeck process.
