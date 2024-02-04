Chapter 1: Getting Started with Parallel Computing and Python
*****

Computer system refresh
=====

Instruction flow
-----

A sequence of instructions loaded by a program counter inside the control unit of a CPU.

Data flow
-----

A sequence of data loaded from the memory into the CPU.


Flynn's taxonomy
=====

SISD
-----

This correponds to the normal von Neuman architecture.

MISD
-----

Each (potential different) instruction gets executed with the same data concurrently.

SIMD
-----

One instruction gets executed with multiple data inputs.

MIMD
-----

Each (potential different) instruction gets executed with multiple data inputs. This is where process/thread-based parallelism happened in morden computers.


Memory organization in MIMD
=====

Shared memory
-----

* All processors can access the shared memory in the same way.
* The synchronization is obtained by reading the tasks of various processors and allowing the shared memory.
* A memory location must not be changed by one task while another task accesses it.
* Sharing data among tasks should be fast.


Distributed memory
-----

* Each processor can only address its own memory.
* Synchronization is achieved by the communication between processors.
* Distribution of the data among the processors affect the performance of system.
* The communication protocol is message-passing.

