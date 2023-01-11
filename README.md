# reader_writer_problem
This algorithm is basically to synchronize the processes who are accessing data and modifying it.

# Introduction
If two readers access the object at the same time there is no issue/error. On the contrary, if two writers or a reader and a writer access the object at the same time, there may be problems that may wrongly modify the data.
To solve these problems, a writer should get exclusive access to an object. So it should be such that a writer should lock the resource until its done modifying it but multiple readers should be able to access it at the same time and not lock it when its only reading.

# Tools & Technologies
1. Linux/Ubuntu is used for compilation and execution of the kernel
2. C is use for code implementation
3. K-threads and spin locks are used to tackle the problem and work for the kernel.

# Methodology & Configuration
We implemented the code in C in an editor and then we formed the code to make it run for the kernel configuration by changing a few libraries and commands. We then added a system call for it and configured the kernel. After installing the kernel successfully, we tested out the system call.
