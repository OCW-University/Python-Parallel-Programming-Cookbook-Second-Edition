Chapter 1: Getting Started with Parallel Computing and Python
*****

Computer system refresh
=====

**Instruction flow**: a sequence of instructions loaded by a program counter inside the control unit of a CPU.

**Data flow**: a sequence of data loaded from the memory into the CPU.


Flynn's taxonomy
=====

.. list-table:: Flynn's taxonomy on computer system
   :header-rows: 1

   * - Architecture
     - Instruction flow
     - Data flow
     - Explaination
   * - SISD
     - 1
     - 1
     - This correponds to the normal von Neuman architecture 
     as noted in `nand2tetris <https://www.nand2tetris.org/>`_
   * - MISD
     - m
     - 1
     - Each (potential different) instruction gets executed with the same data concurrently.
   * - SIMD
     - 1
     - m
     - One instruction gets executed with multiple data inputs.
   * - MISD
     - m
     - m
     - Each (potential different) instruction gets executed with multiple data inputs. 
     This is where process/thread-based parallelism happened in morden computers.


Memory organization in MIMD
=====
