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

Shared memory in MIMD
-----
* the memory is same for all processor.
* a memory location must not be changed by one task while another task accesses it.
* sharing data among tasks should be fast.


Distributed memory in MIMD
-----

