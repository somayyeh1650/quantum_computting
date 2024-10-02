# Project description

Quantum computers operate based on the principles of quantum mechanics, using quantum bits (qubits) instead of classical bits.
Qiskit is an open-source software development framework created by IBM for working with quantum computers. It provides tools to write code, simulate quantum circuits, and run quantum algorithms on real quantum hardware by connecting to [qiskit_ibm_runtime](https://docs.quantum.ibm.com/api/qiskit-ibm-runtime/runtime_service), which gives access to IBM’s quantum devices, including those with 100+ qubits. However, to build and test quantum algorithms in a classical simulation environment, the **Qiskit Aer** simulation module offers an important step before running those algorithms on real quantum processors.




This repository uses qiskit to perform some elementary quantum circuits. It is inspired by an online course entitled [Quantum Computing with Qiskit Ultimate Masterclass](https://www.udemy.com/course/quantum-computing-with-ibm-qiskit-ultimate-masterclass/). All the code presented here is simulated using Qiskit Aer, and we do not use Qiskit IBM Runtime.

# Installation instructions
Rather than directly installing Python, we install Miniconda as recommended by instructors of Qiskit. It allows us to create isolated environments so that we can have different versions of Python and packages installed in separate environments without conflicts. 

This video walks you through the process of installing Miniconda:

[https://www.youtube.com/watch?v=dZWz4Gs_BuI](https://www.youtube.com/watch?v=dZWz4Gs_BuI).

To download Miniconda go to the following link:

[https://docs.anaconda.com/miniconda/index.html](https://docs.anaconda.com/miniconda/index.html) 

There are step-by-step instructions on the Miniconda website for installation in different OSs. For Linux users first you need to find out your system’s architecture by running the following command in the terminal 

    uname -m


Afterwards, run the following commands in the terminal, one at a time. In the second command, replace **<my_system’s_architecture>** with your own system architecture.

    mkdir -p ~/miniconda3
    wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-<my_system’s_architecture> -O ~/miniconda3/miniconda.sh
    bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
    rm -rf ~/miniconda3/miniconda.sh


# Set up the Environment

It is always recommended to create a vitual environment to install only the packages we need, making it more lightweight and customizable. For installing the [virtual environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) in conda you can follow the commands :



    conda create –name <my_env>
    conda activate <my_env>

Now in the created env, the first thing is to install pip:

    conda install pip

and using pip install the latest version of Qiskit:

    pip install qiskit 

and for visualization install the following package:

    pip install matplotlib  




# Code
The repository consists of 12 independent codes in the following order:
1. Qiskit basics and single qubit quantum gates
2. Multi qubit quantum gates
3. Constructing quantum circuits with quantum gates
4. Quantum teleportation
5. Superdense coding
6. Deutsch algorithm
7. Deutsch-Jozsa algorithm
8. Bernstein-Vazirani algorithm
9. Simon's algorithm
10. Grover's search
11. Quantum Fourier transform
12. Quantum phase estimation








  


