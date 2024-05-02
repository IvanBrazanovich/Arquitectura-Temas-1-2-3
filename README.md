# Arquitectura-Temas-1-2-3

# Tema 1: 
- **Arquitectura Von Neumann**
    - Central processing unit (CPU) sequentially processes instructions stored in memory.
    - It emphasizes the concept of stored-program computers, where both instructions and data are stored in the computer's memory.
    - **Key Components: ** 
        - Central Processing Unit (CPU):
        - Memory:
        - Input/Output (I/O) Devices:
        - Control Unit:
- **Microprocessor. Microcontroller**
    - **Microprocessor:**
        - Central processing unit (CPU) on a single integrated circuit (IC).
        - Handles processing tasks in computers and other electronic devices.
        - General purpose
        - Examples: Intel Core series, AMD Ryzen series.
    - **Microcontroller:**
        - Specific purpose
        - Integrated circuit containing a CPU, memory, and programmable input/output peripherals.
        - Used in embedded systems, robotics, automotive applications.
        - Examples: Arduino, PIC, AVR.
- **Subroutines**
    - Also known as procedures, functions, or methods.
    - Segments of code that perform specific tasks and can be reused throughout a program.
    - Enhance modularity, readability, and maintainability of code.
    - Called by a program whenever needed and can return a value to the calling code.
- **Low-level languages**
    - Closer to machine code and hardware.
    - Directly manipulates hardware resources.
    - Requires a deeper understanding of computer architecture.
    - Examples: Assembly language, machine code.
- 
- **Técnicas de direccionamiento** 
    - Immediate Addressing
    - Direct Addressing
    - Indirect Addressing
    - Register Addressing
    - Register indirect
    - Stack or implicit
    - Relative Addressing
        - Base or Displacement Addressing
        - Por referencia al programa
        - Por página o yuxtaposición
    - Indexed Addressing
- 
- **Memory** 
    - **Memory**:
        - Fundamental component of computing systems.
        - Essential for storing and retrieving data and instructions.
        - Types include RAM (Random Access Memory) and ROM (Read-Only Memory).
    - **Memory Hierarchy**:
        - Organizational structure of memory in a computer system.
        - Comprises different levels with varying speeds, capacities, and costs.
        - Examples include cache memory, main memory (RAM), and secondary storage (hard drives, SSDs).
    - **Words**:
        - Basic units of data storage in a computer's memory.
        - Typically represented as a fixed number of bits (e.g., 8 bits = 1 byte).
        - Word size varies across computer architectures and influences memory capacity and processing speed.
    - **Addressable Memory**:
        - Ability to locate and access specific memory locations.
        - Each memory cell in a computer's memory has a unique address.
        - Addressable memory size is determined by the number of unique addresses that can be assigned.
    - **Data Storage Units**:
        - Measurement units used to quantify digital data storage capacity.
        - Common units include bits, bytes, kilobytes, megabytes, gigabytes, terabytes, etc.
        - Storage capacity increases exponentially with each unit, from smallest to largest.
    - **Cache:** 
        - High-speed memory located between the CPU and main memory.
        - Used to temporarily store frequently accessed data and instructions, speeding up the computer's performance.
    - **Virtual Memory:** 
        - Technique that extends the computer's physical memory by utilizing secondary storage (e.g., hard disk) as an extension of RAM.
        - Allows the system to run programs larger than the available physical memory by swapping data between RAM and disk storage.
- 
- 
- **I/O** 
    - **I/O in Computer Architecture**:
        - Concept of Input/Output (I/O) in computer systems.
        - Integration of I/O devices with the CPU and memory.
    - **I/O Modules**:
        - Hardware components facilitating communication between CPU/memory and external devices.
        - Examples include interface cards, controllers, and ports.
    - **I/O Operations**:
        - Basic operations involved in I/O, such as reading from and writing to external devices.
        - Handling interrupts and managing data transfer between CPU and peripherals.
    - **I/O Techniques**:
        - Various strategies for efficient I/O operations, such as programmed I/O, interrupt-driven I/O, and Direct Memory Access (DMA).
        - Discussion on pros and cons of each technique in terms of performance and complexity.
        - **Programmed I/O**:
            - CPU directly controls data transfer between I/O device and memory.
            - Simplest technique but can lead to CPU inefficiency due to polling.
        - **Interrupt-Driven I/O**:
            - I/O devices send interrupts to the CPU when ready to transfer data.
            - CPU can perform other tasks while waiting for interrupts, increasing efficiency.
        - **Direct Memory Access (DMA)**:
            - Dedicated DMA controller manages data transfer between memory and I/O devices.
            - Reduces CPU overhead by allowing data transfer without CPU involvement.
            - Commonly used for high-speed data transfer, such as disk I/O and network operations.
- 
- 
# Tema 2
- **Operating System Objectives: **An OS is a program that controls the execution of application programs, and acts as an interface between applications and the computer hardware. It can be thought of as having three objectives: 
    - **Convenience:** An OS aims to simplify computer usage for end-users by providing intuitive interfaces and features.
    - **Efficiency:** It optimizes the utilization of computer system resources to ensure maximum performance and productivity.
    - **Ability to evolve:** An OS should be adaptable to accommodate new functionalities and technologies without disrupting existing services.
- **Operating System Interface:**
    - **Layered Approach:** The hardware-software architecture is structured in layers, abstracting complexities for easier development and interaction.
    - **End User Perspective:** Users interact primarily with applications, abstracted from underlying hardware complexities.
    - **Application Development:** Programmers create applications using high-level programming languages, relying on system utilities and libraries.
    - **System Programs:** Utilities simplify tasks like file management and I/O device control, enhancing development efficiency.
    - **Role of Utilities:** They encapsulate common functions to streamline application development and system management.
    - **Operating System (OS):** Acts as a bridge between applications and hardware, providing a user-friendly environment while managing system resources.
- **Operating System Services:**
    - **Program Development:** Offers tools like editors and debuggers to assist programmers in creating and debugging applications.
    - **Program Execution:** Handles loading, initialization, and scheduling of programs to ensure efficient resource allocation.
    - **I/O Devices Access:** Provides a uniform interface for interacting with various I/O devices, abstracting hardware complexities.
    - **File Access Control:** Manages file access permissions and data integrity, particularly in multi-user environments.
    - **System Access Control:** Regulates access to system resources, ensuring security and resolving resource conflicts.
    - **Error Handling:** Detects and responds to hardware and software errors to maintain system stability and reliability.
    - **Accounting:** Collects usage statistics and performance metrics for system optimization and billing purposes in multi-user environments.
- **Key Interfaces in a Computer System:**
    - **Instruction Set Architecture (ISA):** Defines the machine language instructions accessible to applications and utilities.
    - **Application Binary Interface (ABI):** Specifies the system call interface for ensuring binary portability across different hardware platforms.
    - **Application Programming Interface (API):** Grants access to hardware resources through libraries and high-level language abstractions, facilitating software portability and development.
- **Operating System as Resource Manager:**
    - **Control Mechanism:** The OS regulates the use of computer resources such as CPU time, memory, and I/O devices.
    - **Execution:** While functioning as software executed by the processor, the OS frequently relinquishes control to allow the execution of other programs, before resuming control to manage system operations.
- 
- **Tipos de kernels** 
    - **Kernel Basics**:
        - The kernel is the core component of an operating system that manages hardware resources and facilitates communication between applications and hardware.
        - It loads into memory when the OS boots and remains there until shutdown.
        - Key tasks include memory management, CPU time allocation, and disk management, achieved through system calls and inter-process communication.
    - **Monolithic Kernels**:
        - Execute all OS services within kernel space.
        - Examples: Linux, UNIX, older Windows versions.
        - Unified structure with all functionalities in a single binary file.
        - Efficient communication between components leads to faster performance.
        - **Advantages of Monolithic Kernels**:
            - Efficiency: Faster due to reduced mode switching.
            - Tight integration: Efficient communication between services.
            - Simplicity: Unified structure eases design and debugging.
            - Lower latency: Direct handling of system calls and interrupts.
        - **Disadvantages of Monolithic Kernels**:
            - Stability issues: Bugs or vulnerabilities affect entire system.
            - Security vulnerabilities: Vulnerable services compromise system.
            - Maintenance difficulties: Changes impact entire system.
            - Limited modularity: Adding/removing functionality is complex.
    - **Microkernels**:
        - Keep kernel small, moving most services to user space.
        - Examples: MINIX, QNX.
        - Enhance reliability and security by minimizing privileged code.
        - Communication between services via message passing.
        - **Advantages of Microkernels**:
            - Reliability: Failure in one service doesn’t affect others.
            - Flexibility: Services can be added/removed independently.
            - Modularity: Each service runs independently, aiding maintenance.
            - Portability: Easier to port across hardware architectures.
        - **Disadvantages of Microkernels**:
            - Performance: More context switches between spaces can slow operations.
            - Complexity: More communication and synchronization mechanisms.
            - Development difficulty: Designing communication mechanisms is intricate.
            - Higher resource usage: More communication increases resource consumption.
    - **Hybrid Kernels**:
        - Combine benefits of monolithic and microkernel architectures.
        - Critical services remain in kernel space; non-essential services move to user space.
        - Examples: Windows NT, macOS.
    - **Modular Kernels**:
        - Divided into independent modules for specific functionalities.
        - Modules can be dynamically loaded and unloaded.
        - Provides flexibility, extensibility, and easier maintenance.
        - Examples: Linux, macOS, Solaris, Windows.
- 
- 
  # Tema 3:
- **Process Definition:**
    - A program in execution, running on a computer.
    - An entity that can be assigned to and executed on a processor.
    - Characterized by a sequence of instructions, a current state, and associated system resources.
    - Composed of program code and data.
- **Process Control Block (PCB) Structure:**
    - Identifier, state, priority, program counter, memory pointers, context data, I/O status information, accounting information.
    - Stored by the OS to manage processes and facilitate interruption and resumption.
- **Process States:**
    - Running: Currently executing process.
    - Ready: Prepared to execute when given the opportunity.
    - Blocked/Waiting: Cannot execute until a specific event occurs.
    - New: Just created, not yet admitted to the pool of executable processes.
    - Exit: Released from the pool of executable processes, either halted or aborted.
- **Dispatcher:**
    - Manages CPU switching between processes.
    - Saves and loads process information.
- **Process Description:**
    - OS manages processes, allocates resources, responds to requests.
- **Process Creation and Termination:**
    - Initialization, allocation of PCB, memory, address space, loading program, resource assignment, registration, notification, execution handoff.
- **Suspended Processes:**
    - Temporarily halted processes.
    - Reasons include waiting for user input, I/O operations, resource availability, or OS scheduling.
- **Process Control:**
    - Management and coordination of processes within an OS.
- **Modes of Execution:**
    - User mode: Executes non-privileged code.
    - Kernel mode: Executes privileged instructions, manages system resources.
- **Process Switching:**
    - Context saving, loading, and execution switching between processes.
- **Stack and Heap (Processes):**
    - Stack: LIFO memory for function contexts and local variables.
    - Heap: Dynamic memory allocation region for larger, flexible memory usage.
    - 
- 
- **Threads** 
- **Program**:
    - Definition: A set of instructions in a programming language for a specific task.
    - Characteristics:
        - Static Nature
        - Executable Code
        - Stored on Disk
        - Doesn't Consume System Resources Until Execution
- **Process**:
    - Definition: The dynamic execution of a program.
    - Characteristics:
        - Dynamic Nature
        - Resource Utilization
        - Has an Identity (Process ID)
        - Can Create Child Processes
        - Can Interact with Other Processes
- **Thread**:
    - Definition: Smallest unit of execution within a process.
    - Characteristics:
        - Subset of the process
        - Lightweight process
        - Shares resources with the process
        - Allows for concurrent execution
        - Shares memory space with other threads in the same process
- **Multithreading**:
    - Single-threading vs. Multi-threading
        - Single-threading: One execution path, tasks executed sequentially.
        - Multi-threading: Multiple threads run concurrently within the same process.
    - Advantages of Multithreading:
        - Concurrency
        - Responsiveness
        - Parallelism
        - Asynchronous I/O
        - Modularization
        - Resource Sharing
        - Event Handling
- **Thread States**:
    - Running, Ready, Blocked
    - Spawn, Block, Unblock, Finish
- **Types of Threads**:
    - User-Level Threads (ULTs)
        - Managed by user-level thread libraries
        - Faster context switching, less responsive when one thread blocks
        - More portable
    - Kernel-Level Threads (KLTs)
        - Managed by the operating system kernel
        - Slower context switching, better responsiveness
        - Less portable, but can utilize multi-core processors effectively
- **Multicore Processors**:
    - Definition: Single IC with multiple processing cores
    - Advantages: Increased parallelism, better resource utilization, enhanced multitasking
    - Challenges: Parallelization, scalability, programming complexity
- **Relationship between Multicore and Multithreading**:
    - Complementary technologies enhancing system performance and responsiveness
    - Multicore processors provide hardware platform for concurrent execution
    - Multithreading allows software to fully utilize multicore processors, improving scalability and responsiveness.
- 
- **Process Scheduling:** 
    - **Types of Processor Scheduling**:
        - Long-Term Scheduling
        - Medium-Term Scheduling
        - Short-Term Scheduling
    - **Scheduling Algorithms**:
        - Various algorithms such as FCFS, SJN, RR, Priority Scheduling are used for short-term scheduling.
    - **Short-Term Scheduling Criteria**:
        - CPU Utilization
        - Turnaround Time
        - Waiting Time
        - Throughput
        - Response Time
    - **The Use of Priorities**:
        - Process priority determines the order of execution.
        - Can lead to starvation issues if not managed properly.
        - Selection function and decision modes are involved in prioritization.
    - **Alternative Scheduling Policies**:
        - Nonpreemptive Scheduling: Process runs until it voluntarily relinquishes CPU.
        - Preemptive Scheduling: OS can interrupt and move processes based on priority or burst time.
    - **Performance Comparison**:
        - Evaluates scheduling algorithms based on CPU utilization, turnaround time, waiting time, throughput, and response time.
    - **Context**:
        - Process scheduling manages CPU usage in multiprogramming systems.
        - Long-term, medium-term, and short-term scheduling are key components.
        - Prioritization, algorithms, and policies optimize resource utilization and system performance.
        - Gantt charts visualize project schedules, while burst time measures process execution duration.
- **First Come First Serve (FCFS):**
    - **Definition:** FCFS is the simplest operating system scheduling algorithm where the process that requests the CPU first is allocated the CPU first, following a First-In-First-Out (FIFO) queue.
    - **Characteristics:**
        - Supports both non-preemptive and preemptive CPU scheduling.
        - Tasks are executed based on the order of their arrival.
        - Easy to implement and use, but not very efficient in performance.
    - **Advantages:**
        - Easy implementation.
        - Follows a fair "first come, first serve" method.
    - **Disadvantages:**
        - Prone to the convoy effect, where long processes can cause shorter ones to wait excessively.
        - Higher average waiting time compared to other algorithms.
- **Shortest Job First (SJF) or Shortest Process Next (SPN):**
    - **Definition:** SJF is a scheduling process that selects the waiting process with the smallest execution time to execute next, aiming to minimize average waiting time.
    - **Characteristics:**
        - Uses the shortest CPU burst time as the main criterion.
        - May cause starvation for longer processes if shorter ones continuously arrive.
    - **Advantages:**
        - Reduces average waiting time compared to FCFS.
        - Suitable for long-term scheduling.
    - **Disadvantages:**
        - Potential for process starvation.
        - Difficulty in predicting the length of upcoming CPU requests.
- **Round-Robin Scheduling (RR):**
    - **Definition:** RR scheduling is similar to FCFS but with preemption, allowing the system to switch between processes. Each process is given a time quantum to execute before being preempted.
    - **Characteristics:**
        - Fair and starvation-free.
        - Preemptive, ensuring each process gets CPU time in a round-robin fashion.
    - **Advantages:**
        - Fairness in CPU allocation.
        - Allows for time-sharing and equal opportunity for all jobs.
    - **Disadvantages:**
        - Larger waiting and response times.
        - Low throughput and increased context switches.
- **Shortest Remaining Time First (SRTF) or Preemptive Shortest Job Next (PSJN):**
    - **Definition:** SRTF is the preemptive version of SJF, where the process with the smallest remaining time until completion is selected to execute next.
    - **Characteristics:**
        - Faster processing of jobs compared to SJF.
        - More context switches, impacting CPU time for processing.
    - **Advantages:**
        - Fast processing of short processes.
        - Low overhead since decisions are made only when processes complete or new ones are added.
    - **Disadvantages:**
        - Potential for process starvation.
        - Long processes may be indefinitely delayed by short processes.
- **Highest Response Ratio Next (HRRN):**
    - **Definition:** HRRN is a non-preemptive scheduling algorithm that selects the process with the highest response ratio, aiming to optimize performance.
    - **Characteristics:**
        - Uses response ratio to prioritize processes.
        - Addresses the starvation issue of SJF.
    - **Advantages:**
        - Better performance than SJF.
        - Reduces waiting time for longer jobs and encourages shorter jobs.
    - **Disadvantages:**
        - Implementation complexity due to the need for burst time prediction.
        - Potential CPU overload.
- **Multilevel Feedback Queue Scheduling (MLFQ):**
    - **Definition:** MLFQ manages process execution in a multitasking environment by assigning processes to multiple queues based on priority and adjusting priorities dynamically.
    - **Characteristics:**
        - Processes can move between queues based on their behavior.
        - Utilizes a feedback mechanism to adjust priorities.
    - **Advantages:**
        - Flexibility in handling different types of processes.
        - Prevents starvation by adjusting priorities dynamically.
    - **Disadvantages:**
        - Complex implementation and selection of the best scheduler.
        - Increased CPU overhead.
- 
- 
- **Sincronización** 
- **Comunicación entre procesos (Interprocess Communication)**:
    - Refiere a la transferencia de datos entre dos o más procesos en un sistema computacional.
    - Es fundamental para la coordinación y cooperación entre procesos, permitiendo la sincronización y el intercambio de información.
- **Procesos Concurrentes (Concurrent Processes)**:
    - Son procesos que ejecutan simultáneamente en un sistema.
    - Pueden compartir recursos y comunicarse entre sí.
    - La concurrencia es esencial para mejorar el rendimiento y la eficiencia del sistema, permitiendo la ejecución paralela de tareas.
- **Condiciones de competencia (Race Conditions)**:
    - Ocurren cuando múltiples procesos o hilos acceden a datos compartidos y el resultado final depende del momento relativo de su ejecución.
    - Pueden provocar resultados inesperados y errores en el sistema si no se gestionan correctamente.
- **Secciones críticas (Critical Sections)**:
    - Son partes de código dentro de un proceso que acceden a recursos compartidos.
    - Deben ejecutarse de manera exclusiva para garantizar la consistencia de los datos y evitar condiciones de carrera.
- **Exclusión mutua con espera ocupada (Busy Waiting)**:
    - Método de exclusión mutua en el que un proceso espera continuamente hasta que otro proceso libere un recurso.
    - Ineficiente ya que consume recursos de CPU sin realizar trabajo útil.
- **Dormir y despertar (Sleep and Wakeup)**:
    - Técnica para evitar la espera ocupada al bloquear un proceso hasta que se cumpla una condición específica.
    - Utiliza llamadas al sistema para suspender y reanudar la ejecución de procesos de manera eficiente.
- **Semáforos (Semaphores)**:
    - Variables de sincronización utilizadas para controlar el acceso a recursos compartidos entre procesos.
    - Pueden ser enteros o binarios y se utilizan para garantizar la exclusión mutua y la sincronización entre procesos.
- **Monitores (Monitors)**:
    - Abstracción de alto nivel que simplifica la sincronización entre procesos al proporcionar un entorno seguro para el acceso a recursos compartidos.
    - Ofrecen mutual exclusión, variables de condición y encapsulación de datos en una sola estructura.
    - Se utilizan para estructurar programas concurrentes de manera más clara y segura.
- **Transferencias de mensajes (Message Passing)**:
    - Mecanismo de comunicación entre procesos que implica enviar y recibir mensajes.
    - Se utiliza para compartir datos y coordinar la ejecución de procesos en sistemas distribuidos.



# TEMA 1
Guías y temas
Videos:
Crash course for the first part
https://youtu.be/n31IHq2FnN8?feature=shared (Arquitectura VN)
https://youtu.be/ii4-MCNE0zs?feature=shared (Direccionamientos parte 1)
https://youtu.be/y4Lnl6B7Sxo?feature=shared (Direccionamiento parte 2)
https://youtu.be/aUB80lCfnyA?feature=shared (Memorias)
Subrutinas - YouTube subrutinas

Temas:  La Computadora, Arquitectura de Von Neumann. Microprocesadores, subrutinas y lenguajes de bajo nivel . Técnicas de Direccionamientos . Memorias . Entrada y Salida. Subrutinas.
# How are the basics of a computer built?

### Note
The foundational components of a computer system are constructed using logic gates, including the CPU, Control Unit, ALU, RAM, etc.

![Computer Basics](https://remnote-user-data.s3.amazonaws.com/4OeCqQT_EeSQ_jMDz2c-d4UDvUSSowcr38ppQXpC7z6bhOR4goEB-YSoQZedkBP1bBCGUbER1RvJUw3OmH28vw9ftlpe7NqSXHvW4Ci9YO3q1P3WMy_Z1a6uZcENVAOi.png)

## How do transistors work?
Transistors function as switches in computer systems, controlling the flow of electronic signals. They operate by opening and closing electronic gates rapidly. When a transistor is turned on, current flows through the circuit; when it's off, current is blocked.

Transistors consist of doped silicon, which alters its conductivity. By applying voltage to specific regions, electrons can be made to flow or be blocked, facilitating the control of current.

![Transistors](https://remnote-user-data.s3.amazonaws.com/C7o-5sjHu0ra-79qlYsxBU2VDpp9LVY_vRXq3g41pJBkyxXWzZvs-1uiiTgG-KNYHuZjryuAzEy5EnnwFAg7ka9Bi0digC-ToU9_Wuw_kP2XWNkAtSccFENGnCoVXsqG.png)

## Boolean algebra and logic gates
Boolean algebra is implemented using transistors to create logic gates, which perform logical operations such as AND, OR, and NOT.

### NOT gate
![NOT Gate](https://remnote-user-data.s3.amazonaws.com/xUpbWC70XQUMPaxwx4BYGMFknMCtM7kRcGJv57sb1iOhM6K8cyd6fg-FJvk7zH9hmzHgTYrOATojv8A6lheP9_wGkZ2DjRQRtL-pw93GisqZP6Wq2n4yyXG8kKW7KmVo.png)

### AND gate
![AND Gate](https://remnote-user-data.s3.amazonaws.com/boozw1wBgyjRv9RbdpHopF5fi8JP7JU30hZueCxcbHXmiHtemoFvjmeSk1957yPyV26DfAtSk3nL2zHu5-DXLYxVxj6W2N_MzGN2QQnyuuBTEMrXzDEOLUVEY7-QDdQQ.png)

### OR gate
![OR Gate](https://remnote-user-data.s3.amazonaws.com/s9ACvzvmcfQ5dLrA6n-IEgrnYJU0C36ZxiyTd1ADqDWu4-gF7nUMCNzJGt6c0_4ohj1sLz1EcryRHaU814arTxRLTNpuvXLICoyCr9fh4ChJ4vPpVzYY3qiDxBBc6kLx.png)

### Exclusive OR (XOR)
![XOR Gate](https://remnote-user-data.s3.amazonaws.com/g9ldKfpqe7J1cjV8nTLjsHjfcNEcqPKHPla4_7A_i3N27lLfwB3iHf1556f9b5OzeaUVwu0jLGvGw05iG1-TB_Fl30EdebEjRwjOWNYioRQM4JqR91FyxpbJ4zgi3h-3.png)

## Representing numbers and letters with binary

Binary notation is crucial for representing numbers and letters in computers. It operates on a base-2 system, where each digit's position represents a power of 2.

1. Base-2 Notation (Binary):
    - Binary digits represent powers of 2, with each digit being either 0 or 1.
2. Possible Digits:
    - Binary digits are limited to 0 and 1.
3. Possible Combinations:
    - The number of combinations in a binary number of length n is 2^n.
4. Example:
    - A 4-digit binary number has 16 possible combinations.

Binary notation is fundamental for digital systems and provides the basis for computer operations. Additionally, decimal notation, based on powers of 10, is essential for everyday arithmetic.

![Binary & Decimal](https://remnote-user-data.s3.amazonaws.com/TaQI8gbdtdfoUFplWrUyeQv6OlVtRo1ZlEX9gYTp3xKjNGRR_sl_TLmW4gvzMT2azU9Wyjl-MiDPfIm5M2k-erWW8xLnmEU8ExWopNAJ0tzs3aBu6VwuqTXx2-NTY3Zo.png)

In computer systems, binary is commonly used to represent data. For example, a byte consists of 8 bits, allowing for 256 possible combinations. Binary notation, along with logical operations, forms the basis of computer arithmetic and data representation.

# Numbers, Letters, and Arithmetic Logic Units (ALUs)

## Representation of Numbers and Letters
- **Floating Numbers**: Represented in memory to include numbers with commas.
- **Letters**: Represented with numerical values using ASCII and Unicode encoding standards.

### ASCII
- Utilizes 7 bits, allowing for 128 possible combinations.
- Assigns numerical values (0 to 127) to characters, primarily for English text.

### Unicode
- Character encoding standard supporting characters from all languages and writing systems.
- Assigns unique numerical values to each character, using 16 bits.

## Arithmetic Logic Unit (ALU)
- Component of a computer's CPU performing arithmetic and logical operations on data.
- Operations include addition, subtraction, multiplication, division, AND, OR, and NOT.
- ALU consists of arithmetic and logic units.

### Arithmetic Unit
- Handles numerical operations in a computer.
- Addition operation in binary represented by a half-adder circuit.
  ![Half Adder Circuit](https://remnote-user-data.s3.amazonaws.com/JvRJd59EtwAUMpy6uhL7FXDgwy0apF2piOBiUnNVf4Q_zcl8_anG8n7XY2l4URDhrLWMLx3n7fkbMHQkGdCUN05TPrJm7Y0D4by6jyW8dTEp5pyoLmXfWH_G0jNiuW1H.png)
- Full-adder circuit needed for adding numbers with carries.

### Logic Unit
- Performs logical operations like AND, OR, and NOT on binary inputs.
- Essential for decision-making and data manipulation during computations.

# Registers, RAM, and Memory Addressing

## Logic Circuits for Memory
- Two useful circuits: AND-OR latch and gated latch.
- Used for saving data and creating memory, essential components of RAM.

### AND-OR Latch
- Saves 0 or 1 into a circuit, basic unit of memory.

### Gated Latch
- Allows control over data storage with write enable circuit.

## Memory Addressing
- Data stored in latches with addresses for access.
- Addressing managed by multiplexers, enabling row and column selection.

### Matrix Memory
- Matrix of latches used for scalable memory storage.
- Utilizes shared wires for addressing and data transfer, minimizing wiring.

## Random Access Memory (RAM)
- Temporary storage for data and instructions required by the CPU.
- Facilitates rapid data retrieval and storage, crucial for program execution.

# Central Processing Unit (CPU) and Program Execution

## CPU Components
- RAM stick, memory registers, instruction address register (IAR), and instruction register (IR).

### CPU Registers
- Temporary storage for manipulating values during program execution.

## CPU Operation Phases
1. **Fetch Phase**:
   - Retrieves instructions from RAM based on IAR.
2. **Decode Phase**:
   - Interprets binary instruction code, extracting opcode and data address.
3. **Execute Phase**:
   - Carries out the operation specified by the decoded instruction.

This cycle repeats, enabling the CPU to execute a series of instructions and perform complex computations required by the program.


Example step by step:
Assumptions:
The CPU has separate registers for A, B, and an Instruction Register (IR).
The RAM is used to store both data and instructions.
The ALU (Arithmetic Logic Unit) performs arithmetic operations.

1. LOAD_A:
Clock cycle 1-3:
    Fetch:
        The Instruction Address Register (IAR) contains the address of the next instruction.
        The Control Unit fetches the instruction from the RAM at the address specified by the IAR.
        The fetched instruction is stored in the Instruction Register (IR).
    Decode:
        The Control Unit interprets the instruction in the IR as LOAD_A.
        It sets the necessary control signals to prepare for executing this instruction.
    Execute:
        The Control Unit signals the RAM to fetch the data from the memory address specified in the instruction.
        The data is loaded into the A register.
https://remnote-user-data.s3.amazonaws.com/2nOjcZwb5Ao6nLQwzsfJT7y_CoP8JJbV1oY_8u8V1Yzku-fi68Q0t-YQLkMP9jcyPF3DdccZPOq0QNL9jObm9sqcSHVNLCvFijmUGyVYvWIoRdkVsTPU0pvOJt6cQBQ9.png

2. LOAD_B:
Clock cycle 4-6:
    Fetch:
        The Control Unit increments the IAR to point to the next instruction.
        It fetches the next instruction from RAM into the IR.
    Decode:
        The Control Unit identifies the instruction as LOAD_B.
        Control signals are set accordingly.
    Execute:
        The Control Unit instructs the RAM to retrieve the data from the specified memory address.
        The retrieved data is loaded into the B register
The same as the image before but with register B
3. ADD:
Clock cycle 7-9:
    Fetch:
        The Control Unit increments the IAR to get the next instruction.
        It fetches the instruction from RAM into the IR.
    Decode:
        The Control Unit recognizes the instruction as ADD.
        In this case we have a 2 2-bit RAM ADDRESS (look up in the operations code list), which means that we can select 2 of the 4 registers we have. The first 2-bits for the register B and the next for the A.
        Necessary control signals are set.
    Execute:
        The Control unit enables register b and feeds its value to input 1
        The Control unit enables register a and feeds its value to input 2
        The control unit configures the ALU passing the operation code
        The output goes to a temporary memory register inside the Control unit
        The control unit stores the register A value

https://remnote-user-data.s3.amazonaws.com/OyfIXn-nMOmM5LF820PSZ5w2pGab2wWphXF9GVHj7ytMpMWZWeRRGPTZIfvcOr61vCFFoIHqY1LWCWfCfQpKXuiWb9VEjT56zJBlcufSkaZmsG5OW2INclsy2XI6sHHO.png

4. STORE_A:
Clock cycle 10-12:
    Fetch:
        The Control Unit increments the IAR.
        It fetches the next instruction from RAM into the IR.
    Decode:
        The Control Unit identifies the instruction as STORE_A.
        Control signals are set accordingly.
    Execute:
        The Control Unit instructs the RAM to store the content of register A into the specified memory address.
At the end of the execution, the process is complete, and the result of the addition is stored in RAM or any other specified location. This sequence demonstrates the fundamental steps involved in executing instructions on a simple 8-bit CPU with RAM. Each instruction goes through fetch, decode, and execute phases, with one action per stage.

What is the control unit of a cpu?  
The control unit is a crucial component of a CPU (Central Processing Unit). It's responsible for coordinating the activities of the other hardware components within the CPU and ensuring that instructions from computer programs are executed in the correct sequence.
Here are some key points about the control unit:
1. Instruction Interpretation: The control unit interprets the instructions fetched from memory during the fetch phase of the CPU cycle. It decodes these instructions to determine the specific operation that needs to be performed.
2. Instruction Execution: Once instructions are decoded, the control unit coordinates the execution of these instructions. It directs the necessary arithmetic, logical, or data transfer operations within the CPU to carry out the instruction's specified task.
3. Sequencing and Timing: The control unit manages the sequencing and timing of operations within the CPU. It ensures that instructions are executed in the correct order and that each operation occurs at the appropriate time.
4. Control Signals: The control unit generates control signals that regulate the flow of data between different CPU components, such as registers, ALU (Arithmetic Logic Unit), and memory. These control signals facilitate the movement of data and the execution of instructions.
5. Synchronization: In multi-core CPUs, where multiple processing cores are present, the control unit helps synchronize the activities of these cores to ensure efficient processing and avoid conflicts between tasks.
Overall, the control unit acts as the "brain" of the CPU, orchestrating its various components to execute instructions and perform computations according to the program's requirements. It plays a crucial role in the overall functioning and performance of the CPU.




CPU's clock  
The "clock" of a CPU refers to its internal timing mechanism, which regulates the rate at which the CPU executes instructions. This clock signal sets the pace for the CPU's operation, defining the intervals at which it processes data and executes instructions. The clock speed, usually measured in hertz (Hz), represents the frequency at which this internal clock oscillates.
For example, if a CPU has a clock speed of 3.0 gigahertz (GHz), it means that the internal clock of the CPU cycles at a rate of 3.0 billion times per second. Each cycle of the clock typically corresponds to a basic unit of work that the CPU can perform, such as fetching an instruction, decoding it, executing it, and storing the result.

Other definitions
1. Clock Signal: The CPU's clock signal is a regular, periodic waveform that oscillates between high and low voltage states at a constant frequency. This frequency, measured in Hertz (Hz), determines the rate at which operations are synchronized and controlled within the CPU.
The clock signal sets the rhythm or pace at which the CPU operates. It determines the timing and frequency of execution, effectively dividing time into discrete intervals or cycles. Each cycle corresponds to a specific amount of time during which a set of operations can occur.
2. Clock Cycle: The clock cycle represents one complete pulse of the CPU's clock signal. It defines the basic unit of time for the CPU's operations and sets the pace at which instructions are processed.
3. Pipeline: The CPU's pipeline breaks down the execution of instructions into multiple stages, such as fetch, decode, execute, and write back. Each stage of the pipeline represents a distinct operation or task within the instruction processing cycle. This allows to execute more than one action at a time. Instructions  that would usually take 3 (or more, depending on the cpu) stages, don't finish before the next instruction is fetched, rather the cpu moves the fetched instruction to the decode phase, and fetches a new instruction, creating a flow in the pipeline.
https://remnote-user-data.s3.amazonaws.com/FS1rkk4Yd55IuP80FME2qdwrO-Qq-l_pD4oFWwNoKrleCYmFttZBPrYqKJKFWUy39sk2rXzu7clUn4Sgy1eiZzvst35EAspsZtm23-X6iu98wApejh7gTHY8mCuDDigT.png
4. Concurrency: Within the pipeline, multiple instructions can be in different stages of execution simultaneously, allowing for overlap and parallelism of operations. This concurrency helps improve CPU efficiency and throughput.
5. Pipeline Stalls: When an operation within the pipeline takes longer than a single clock cycle to complete, the pipeline may stall or pause temporarily. During a stall, the pipeline remains idle until the lengthy operation finishes, maintaining synchronization with the CPU's clock signal.
6. Clock Frequency and Performance: The CPU's clock frequency, combined with the efficiency of its architecture and pipeline design, determines its overall performance. Higher clock frequencies generally allow for faster instruction processing, while efficient pipelining and optimization techniques help maximize CPU throughput and efficiency.


La Computadora, Arquitectura de Von Neumann
Summary  
The Von Neumann architecture, named after Hungarian-American mathematician and physicist John von Neumann, is a theoretical framework for a computer's design that is still widely used today. It's the basis for almost all modern computers, including desktops, laptops, smartphones, and servers.
The key components of the Von Neumann architecture are:
1. Central Processing Unit (CPU): This is the brain of the computer. It executes instructions fetched from memory, performs arithmetic and logic operations, and controls the flow of data within the system.
2. Memory: In the Von Neumann architecture, both instructions and data are stored in the same memory unit. This memory is typically divided into two types: RAM (Random Access Memory) for temporary storage of data and instructions currently being processed by the CPU, and storage (such as a hard drive or solid-state drive) for long-term storage of data and programs.
3. Control Unit (CU): The control unit manages the flow of instructions within the CPU. It fetches instructions from memory, decodes them, and executes them in sequence.
4. Arithmetic Logic Unit (ALU): This component performs arithmetic and logic operations on data. It's responsible for tasks like addition, subtraction, multiplication, division, and comparisons.
5. Input/Output (I/O) System: This system handles communication between the computer and external devices, such as keyboards, mice, monitors, and printers. It allows the computer to send and receive data to and from these devices.
The Von Neumann architecture is characterized by its "stored-program concept," which means that both program instructions and data are stored in memory, and the CPU fetches instructions from memory sequentially to execute them. This is in contrast to earlier computing models where programs were hard-wired into the machine and couldn't be easily changed.
One of the main advantages of the Von Neumann architecture is its flexibility. Since programs and data are stored in the same memory, it's relatively easy to write new programs and modify existing ones. This makes it well-suited for general-purpose computing tasks.
However, this architecture also has limitations. For example, the Von Neumann bottleneck refers to the fact that the CPU can only fetch and execute one instruction at a time, which can limit performance in some scenarios. Additionally, the shared memory design can lead to security vulnerabilities, as it's possible for malicious programs to alter the instructions being executed or access sensitive data in memory.
Overall, the Von Neumann architecture is a fundamental concept in computer science and serves as the basis for understanding how modern computers are designed and operate.
https://remnote-user-data.s3.amazonaws.com/cn0A6m7ARvY-SyQyzHlGtSh4gJmsnJFL2pfM5D26_0VT3J5enHiXe2XBujEesR3UyFjVHF6AZ58cVihnoXimFAkEtvzciSH83d9n6i6FmPJHedSthOkcfP5HxelNkDx9.svg

Development  
The first generation of computers utilized vacuum tubes for digital logic elements and memory. The IAS computer, a prominent first-generation computer, introduced the stored-program concept, attributed to mathematician John von Neumann and concurrently developed by Alan Turing. This concept was first proposed in von Neumann's 1945 EDVAC proposal. The IAS computer was designed by von Neumann and his colleagues at the Princeton Institute for Advanced Studies, completed in 1952, and served as the blueprint for subsequent general-purpose computers.
The structure of the IAS computer includes: 
Main memory storing both data and instructions.
An arithmetic and logic unit (ALU) capable of binary data operations.
A control unit interpreting and executing instructions stored in memory.
Input-output (I/O) equipment operated by the control unit.


https://remnote-user-data.s3.amazonaws.com/ITRrv7EjO2WjKQvxDALnOcUtF_nunZPWBEBGfT1ukQO3kgCjIhG8DGZYXFqr0vzMOZVF6Zo2LBSt1vbZ_jl3MRgyWCSBCGvb7JcuvfEPBpyUkGjK_S5rUKUHZBRevtaV.png
Memory Buffer Register (MBR):
    Contains a word to be stored in memory or sent to the I/O unit.
    Used to receive a word from memory or from the I/O unit.
Memory Address Register (MAR):
    Specifies the address in memory of the word to be written from or read into the MBR.
Instruction Register (IR):
    Contains the 8-bit opcode instruction being executed.
Instruction Buffer Register (IBR):
    Employed to temporarily hold the right-hand instruction from a word in memory. The difference between the IBR and the IR is that the IBR fetches the instruction from memory and stores it, that instruction is not being decoded and nothing is being done with it. When the IR is ready to get another instruction, the IBR sends the stored instruction to the IR, where it is decoded, etc.
Program Counter (PC):
    Contains the address of the next instruction pair to be fetched from memory.
Accumulator (AC) and Multiplier Quotient (MQ):
    Employed to temporarily hold operands and results of ALU operations.
    For example, when multiplying two 40-bit numbers, the result is an 80-bit number. The most significant 40 bits are stored in the AC, and the least significant bits are stored in the MQ.



Why does the MBR connect with the I/O processes?  
The I/O (Input/Output) operations often involve transferring data between the CPU and external devices, such as storage units, network interfaces, or peripherals like printers and keyboards. The Memory Buffer Register (MBR) is involved in these operations because it serves as a temporary storage location for data during data transfers between the CPU and memory, or between the CPU and I/O devices.
Here's why the I/O operations work with the MBR:
1. Data Transfer: When data needs to be moved between the CPU and memory or between the CPU and an I/O device, it passes through the MBR. The MBR acts as a buffer, temporarily holding the data during the transfer process.
2. Versatility: The MBR is designed to handle various types of data transfers. It can store data that is being read from memory or an I/O device before it's processed by the CPU. Similarly, it can hold data that the CPU wants to write into memory or send to an I/O device.
3. Interface: The MBR serves as an interface between different components of the computer system. It allows the CPU to communicate with memory and I/O devices efficiently by providing a standardized location for data to be temporarily stored during transfer operations.
4. Efficiency: By using the MBR as an intermediate storage location, the CPU can continue executing instructions while data transfers are in progress. This improves overall system efficiency by minimizing the idle time of the CPU.
In summary, the MBR is an integral part of the data transfer process in a computer system, serving as a temporary storage location for data during I/O operations between the CPU, memory, and external devices.







How do the MBR and MAR work together?  
The Memory Buffer Register (MBR) and Memory Address Register (MAR) work together in the process of transferring data between the CPU and memory in a computer system.
Here's how they collaborate:
1. Data Transfer Initialization:
    When the CPU needs to read data from or write data to a specific memory location, it first loads the memory address into the MAR. The MAR holds the address of the memory location where the data transfer will occur.
2. Data Transfer Execution:
    Once the memory address is loaded into the MAR, the CPU initiates the data transfer process. The data to be transferred is either fetched from memory or sent to memory, depending on the operation being performed.
    During this process, the MBR serves as a temporary storage location for the data being transferred. If data is being read from memory, it is temporarily stored in the MBR before being processed by the CPU. Similarly, if data is being written to memory, it is first loaded into the MBR before being written to the specified memory location.
3. Completion and Result:
    After the data transfer is completed, the CPU can access the data in the MBR for further processing, such as arithmetic or logic operations.
    Once the operation is complete, the CPU may update the contents of the MBR or MAR as necessary for subsequent operations.
In summary, the MAR is responsible for holding the memory address where data is to be read from or written to, while the MBR acts as a temporary storage location for the data during the transfer process. Together, they facilitate efficient data transfer between the CPU and memory in a computer system.

Microprocesadores, subrutinas y lenguajes de bajo nivel 
Microprocessors
Fundamental Components of a Digital Computer:  
The basic elements of a digital computer, as we know, must perform data storage, movement, processing, and control functions. Only two fundamental types of components are required: gates and memory cells.
Gates: These devices execute Boolean or logical functions, controlling the flow of data similar to canal gates. Example: An AND gate produces output based on the truth values of its inputs (A and B).
Memory Cells: Responsible for storing binary data, each capable of holding a single bit in two stable states. There are many types, the function is just to store data.

Functions:
Data Storage: Handled by memory cells.
Data Processing: Executed by gates, manipulating data based on input signals.
Data Movement: Enabled through pathways connecting memory cells and gates, facilitating information transfer.
Control: The paths among components can carry control signals. For example, a gate will have one or two data inputs plus a control signal input that activatesthe gate. When the control signal is ON, the gate performs its function on thedata inputs and produces a data output. Conversely, when the control signalis OFF, the output line is null, such as the one produced by a high impedance state. Similarly, the memory cell will store the bit that is on its input lead when the WRITE control signal is ON and will place the bit that is in the cell on its  output lead when the READ control signal is ON.  PEDIRLE EXPLICACIÓN AL PROFESOR
https://remnote-user-data.s3.amazonaws.com/mNmzUwKODjSzRnHtD-LJqnsCwrjFfwlNQivsNd8a5k-oR8x9tr7JyAL9rZIubCeKzvYp6LBtj-6YObmg6O6YzwoRyNrV3OSiucLo2qZodf1EC_g9rB5BbByFJciFJ1n8.png
https://remnote-user-data.s3.amazonaws.com/SkaJWDwysqHQOMrZV0tWoBk0plSkup7FNDZjDs5JFLiKdlB4zcOYnpdFGVx47Nw6ZQYSgRDcagWk5DK0C-PcSekSNe00Oh4F4vf8OWnBrcQf7-oQYy0wRwPGt7-Ad-MI.png

What is a microprocessor? 
A microprocessor is a type of processor that contains all the components of a central processing unit (CPU) on a single chip. It is capable of executing general-purpose computing tasks and has evolved over time to become increasingly powerful and versatile.
Before the advent of microprocessors, CPUs (Central Processing Units) were typically constructed using discrete components, meaning individual transistors, diodes, resistors, and other electronic components were assembled together on a circuit board to create the CPU's logic and processing functions. These CPUs were often large, power-hungry, and relatively slow compared to modern microprocessors.
The Intel 8080 was the first general-purpose microprocessor. Introduced in 1974, it was designed to serve as the CPU for a wide range of computing applications, rather than being tailored to a specific use case like its predecessors. The 8080 offered improved performance, a larger instruction set, and greater versatility compared to earlier microprocessors such as the Intel 4004 and 8008, which were designed for specific applications like calculators and embedded systems. The Intel 8080 played a crucial role in the development of early personal computers and is considered a landmark in the history of microprocessor technology.

Microcontroller vs microprocessor  
1. Microcontroller:
    A microcontroller is a compact integrated circuit designed to perform specific tasks within a larger system.
    Microcontrollers are often used in embedded systems where the application requires a dedicated and optimized control mechanism.
    They are commonly found in devices such as washing machines, microwave ovens, remote controls, automotive systems, and various IoT devices.
    Microcontrollers are designed to execute specific tasks efficiently with minimal power consumption and cost.
2. Microprocessor:
    It primarily focuses on executing instructions and performing arithmetic and logical operations.
    Microprocessors are commonly found in general-purpose computing devices such as personal computers, servers, laptops, tablets, and smartphones.
    They are designed to provide high performance and versatility, suitable for a wide range of applications.

Things to know: microprocessors (maybe?)
1. Architecture: Understand the basic architecture of a microprocessor, including components such as the arithmetic logic unit (ALU), control unit, registers, and data bus. Familiarize yourself with concepts like instruction fetching, decoding, and execution.
2. Instruction Set Architecture (ISA): Learn about different instruction sets such as Reduced Instruction Set Computing (RISC) and Complex Instruction Set Computing (CISC). Understand the types of instructions, addressing modes, and how instructions are encoded.
3. Registers: Know the purpose and types of registers in a microprocessor, including general-purpose registers, special-purpose registers (like program counter, instruction register, stack pointer), and status flags.
4. Memory: Understand how microprocessors access memory, including concepts like memory addressing, memory hierarchy (cache, RAM, ROM), and memory management techniques (virtual memory, paging).
5. Pipeline: Learn about instruction pipelining and how it enhances processor performance by overlapping instruction execution stages. Understand pipeline hazards and techniques to mitigate them (such as forwarding and stalling).
6. Interrupts and Exceptions: Understand how interrupts and exceptions are handled by the microprocessor. Learn about interrupt vectors, interrupt prioritization, and exception handling mechanisms.
7. Clock and Timing: Understand the role of the system clock in synchronizing operations within the microprocessor. Learn about clock frequency, clock cycles, and how they impact the performance of the processor.
8. Parallelism: Familiarize yourself with concepts of parallel processing, including instruction-level parallelism (ILP), thread-level parallelism (TLP), and multi-core architectures. Understand techniques such as pipelining, superscalar execution, and SIMD (Single Instruction, Multiple Data) processing.
9. Peripheral Interfaces: Know about various peripheral interfaces commonly used with microprocessors, such as UART, SPI, I2C, USB, and Ethernet. Understand how these interfaces facilitate communication with external devices.
10. Application Areas: Explore the diverse application areas of microprocessors, including personal computing, embedded systems, networking equipment, industrial automation, automotive electronics, and IoT devices.
11. Development Tools: Familiarize yourself with development tools and environments used for microprocessor programming and debugging, such as assemblers, compilers, simulators, and debuggers.
12. Recent Trends: Stay updated on recent advancements and trends in microprocessor design, including topics like power efficiency, security features, heterogeneous computing, and emerging architectures (such as neuromorphic and quantum computing).


Subrutinas
Subroutines on a CPU architecture work by allowing the execution of a block of code separate from the main program flow. Here's a summary of how subroutines function on a CPU:
1. Call:
    When a subroutine is called, the CPU transfers control to the starting address of the subroutine.
    This is typically done using a "call" instruction, which saves the address of the next instruction (the return address) onto the stack before transferring control.
2. Execution:
    The CPU executes the instructions within the subroutine as specified by the program.
    The subroutine may perform various tasks, manipulate data, and execute logic based on its purpose.
3. Return:
    Once the subroutine execution is complete, control is transferred back to the main program.
    This is typically done using a "return" instruction, which retrieves the return address from the stack and resumes execution from that point.
4. Stack Manipulation:
    The CPU often uses a stack to manage subroutine calls and returns.
    The stack is used to store return addresses, parameters, and local variables.
    When a subroutine is called, the return address is pushed onto the stack. When the subroutine returns, the return address is popped from the stack to resume execution.
5. Parameter Passing:
    Subroutines can accept parameters to customize their behavior.
    Parameters may be passed via CPU registers, stack parameters, or a combination of both.
    Parameters are typically passed before calling the subroutine and accessed within the subroutine using specific addressing modes.
6. Local Variables:
    Subroutines may have local variables stored in CPU registers or memory locations.
    Local variables are used to store temporary data needed for the subroutine's execution.
    These variables are often allocated and deallocated within the subroutine's code.
7. Interrupts and Exceptions:
    Subroutines are also used to handle interrupts and exceptions in CPU architectures.
    When an interrupt occurs, control is transferred to a specific interrupt service routine (ISR) subroutine.
    Similarly, exceptions trigger exception handling routines to handle errors or exceptional conditions.
Overall, subroutines allow for modular and structured programming by enabling code reuse, abstraction, and encapsulation of functionality within a CPU architecture. They play a crucial role in organizing and managing program logic at the low-level CPU level.

In low-level CPU architecture, such as assembly language programming, subroutines are still fundamental constructs, although they might be implemented differently compared to higher-level programming languages. At the CPU level, subroutines are typically implemented using concepts like branching, stack manipulation, and the instruction pointer.

how are subroutines  typically implemented at the CPU level?
1. Jump Instructions: CPUs have instructions that allow them to jump to a specific memory address to execute instructions. This is often used to transfer control to the beginning of a subroutine.
2. Call and Return Instructions: CPUs typically have instructions specifically designed for calling and returning from subroutines. The "call" instruction transfers control to a specified memory address, which typically contains the start of the subroutine. The "return" instruction transfers control back to the instruction immediately after the call instruction, effectively returning from the subroutine.
3. Stack Manipulation: CPUs commonly use a stack to manage subroutine calls and returns. When a subroutine is called, the CPU typically pushes the current instruction pointer (the address of the next instruction to be executed) onto the stack. This allows the CPU to return to the correct location after the subroutine finishes executing.
4. Parameter Passing: Parameters can be passed to subroutines in various ways, such as through CPU registers or the stack. For example, in x86 assembly language, parameters are often passed via registers like eax, ebx, etc., or pushed onto the stack before calling the subroutine.
5. Local Variables and Registers: Subroutines may use local variables stored in registers or memory locations reserved for the subroutine's use. Some registers may be designated for specific purposes within subroutines, such as storing return values or other temporary data.
6. Interrupts and Exceptions: Subroutines are also used to handle interrupts and exceptions in CPU architectures. When an interrupt occurs, the CPU typically transfers control to an interrupt service routine (ISR), which is essentially a special type of subroutine designed to handle the interrupt. Similarly, exceptions (such as division by zero or invalid memory access) can trigger exception handling routines.
In assembly language programming, subroutines are often defined using labels to mark the entry and exit points of the subroutine. Jump and call instructions are then used to transfer control between different parts of the program.
Overall, while the implementation details may vary depending on the specific CPU architecture and assembly language, the concept of subroutines remains essential for organizing and managing code at the low-level CPU level.

Lenguajes de bajo nivel
What are Low Level Languages?  
We call those languages as low level languages which are closer to hardware as compared to high-level languages instead of software. They provide little or no abstraction from the machine instructions and that’s why they allow programmers to manipulate hardware elements like register, memory etc. Low-level languages are often used for designing systems, such as developing operating systems, device drivers, and embedded systems.

Types of Low-Level Languages   
Low level language are divided into two types.
Machine Language
    We know that machines follow the language of binary system, means 0 and 1. Machine language is low level language which consists of binary codes which are directly operated by CPU Central Processing Unit. There every instruction are written in form of 0 and 1, so its very challenging for humans to understand and use as primary language.
Assembly Language
Assembly language is a way of writing computer programs that are very close to how the computer works. It have some symbols and codes that represent the basic operations that the computer can perform, which includes adding, moving, or comparing numbers. Because every computer use different architecture for processing so computer have there own instructions so we can say every computer have there own assembly language. It is way higher level language then machine language so its more faster and but still its hard to write and read. To run a program written using assembly language we need to convert it to machine language which is binary . This conversion is done by a program called an assembler.

Languages Examples
x86 Assembly: Commonly used in Intel-based systems, x86 assembly is widely employed for low-level system programming and device drivers.
ARM Assembly: Popular in embedded systems, mobile devices, and IoT applications, ARMassembly language is known for its power efficiency and versatility.
Machine Languages: While machine languages vary between different CPU architectures, they all share the common attribute of consisting of binary code that the CPU can execute directly.
Uses of Low-Level Language  
Low-level programming languages find applications in various fields, including:
Operating System Development: We know that a operating system needs a lot of hardware resources to operate and they must be connected each other in some way. Low level programming languages helps managing hardware resources and allow s using them with control and efficiency.
Embedded Systems: In devices where hardware has to operate directly with on code, like microcontrollers, medical equipment, automotive systems, and IoT devices, low level languages allows us to establish some control over hardware.
Device Drivers: Most of the device drivers such as headphone drivers, speaker drivers are written in low level languages to ensure proper use of hardware, thus facilitating communication between hardware and operating system.
Real-time Systems: There are systems which require performing actions according to time, means require strict timing and minimal response latency for example in aviation control systems and robotics, rely on low-level languages for precise control.
Reverse Engineering: Testingand debugging of hardware and software. Low-level languages allow programmers to directly manipulate the registers and memory of the computer and monitor the execution of instructions. Low-level languages are invaluable for analyzing and understanding the proper functioning of software or malware.
Advantages of Low-Level Languages  
Low level languages provides efficiency to programmers because they allow them to write highly optimised code which can use system resources such as memory, handling CPU cycles very efficiently
Programmers are able manipulate hardware registers and memory locations, enabling precise control over devices, peripherals, and system resources using low level languages
Low level languages lack abstraction means there is very less layers between programmer and hardware which allows programmers to change their code for specific tasks and gain a deep understanding of how the hardware functioning.
Due to direct hardware control of low level languages, they can be used to implement security features and access control mechanisms at a very low level.
Disadvantages of Low-Level Languages  
Writing code in low level languages can be lot harder as compared to high level languages because in these we have to manage memory and registers at real time.
There are low abstraction in low level languages they lack high level abstractions which make programming more accessible and user-friendly.
Code written in low-level languages is often tightly coupled to a specific hardware architecture, that’s why it cannot be used for other platforms devices.
Its take a lot of time for developing a software using low level language because we need to give attention to very small details during this process.
Técnicas de Direccionamiento
The address field or fields in a typical instruction format are relatively small. We would like to be able to reference a large range of locations in main memory or, for some systems, virtual memory. To achieve this objective, a variety of addressing techniques has been employed. They all involve some ­rade-​­ t off between address range and/or addressing flexibility, on the one hand, and the number of memory references in the instruction and/or the complexity of address calculation, on the other. In this section, we examine the most common addressing techniques, or modes:
1. Immediate Mode: In immediate mode, the operand itself is specified directly within the instruction. This means that the data to be operated on is given explicitly in the instruction. For example, in the instruction ADD R1, #5, the value 5 is directly provided in the instruction to be added to the contents of register R1
2. Direct Mode: Direct addressing, also known as absolute addressing, involves specifying the memory address directly within the instruction to access the operand. The CPU directly accesses the data stored at that memory address. For instance, in the instruction LOAD R1, 1000, the value stored at memory address 1000 is loaded into register R1.
3. Indirect Mode: Indirect addressing involves specifying a memory address in the instruction, but instead of directly accessing the data at that address, the CPU retrieves the memory address from that location and then accesses the data from the retrieved address. For example, in the instruction LOAD R1, (R2), the CPU loads the value from the memory address stored in register R2 into register R1.
4 . Register addressing: is similar to direct addressing. The only difference is that the address field refers to a register rather than a main memory address, basically the operand of the instruction is in the register specified:
5. Register Indirect Mode: Register indirect addressing involves specifying a register in the instruction, and the CPU accesses the memory location whose address is contained within that register. For instance, in the instruction LOAD R1, (R2), the CPU accesses the memory location whose address is stored in register R2 and loads the data from that location into register R1.
6. Displacement Mode : Displacement addressing involves adding a constant offset to a base register's value to calculate the effective address of the operand. The offset is often specified as part of the instruction or contained in a register. This mode is useful for accessing elements of arrays or data structures. For example, in the instruction LOAD R1, 100(R2), the CPU loads the value from the memory address obtained by adding 100 to the contents of register R2 into register R1.
Relative addressing
­Base-​­register addressing
Indexing
7. Stack Mode (OR IMPLICIT): Stack addressing involves implicitly using a special-purpose register, typically called the stack pointer (SP), to access operands from the top of the stack. Operations like push and pop are used to add data onto and remove data from the stack, respectively. This mode is commonly used for function calls, local variable storage, and managing program control flow.
These addressing modes provide flexibility in accessing operands and are utilized based on the requirements of specific instructions and programming paradigms. Understanding them is essential for efficient assembly language programming and computer architecture design.
https://remnote-user-data.s3.amazonaws.com/h6923wqhD2S_2GsBcj9Rfk2K5Y8TdjpkCNNPoBlxyyy28Ddc7I5ZRbYiOt54EkG-AnMuxfEk7M4TTQ830Mu_Q9HAAjL0iM7PR2Qn_OuEzC-0T9iqS33KVWxUmHL8Vn78.png
Immediate Mode:
In immediate mode, the operand itself is specified directly within the instruction. This means that the data to be operated on is given explicitly in the instruction. For example, in the instruction ADD R1, #5, the value 5 is directly provided in the instruction to be added to the contents of register R1


Direct Addressing
A very simple form of addressing is direct addressing, in which the address field contains the effective address of the operand:
EA = A
The technique was common in earlier generations of computers but is not com- mon on contemporary architectures. It requires only one memory reference and no special calculation. The obvious limitation is that it provides only a limited addressspace.

Indirect Addressing
With direct addressing, the length of the address field is usually less than the word length, thus limiting the address range. One solution is to have the address field refer to the address of a word in memory, which in turn contains a ­full-length address of the operand. This is known as indirect addressing:
As defined earlier, the parentheses are to be interpreted as meaning contents of. The obvious advantage of this approach is that for a word length of N, an addressspace of 2N is now available (básicamente si cada palabra dentro de un espacio de memoria que vos podés referenciar tiene una longitud de 8 bits, puedes referenciar 2pow8). The disadvantage is that instruction execution requires two memory references to fetch the operand: one to get its address and a second toget its value.
Supongamos que tienes 4 bits, solamente puedes referenciar 16 palabras
Ahora si utilizas indirect addressing y cada palabra tiene 8 bits, si referencias a una palabra, esta puede tener un span de hasta 2pow8 = 256 palabras:


Register addressing:
is similar to direct addressing. The only difference is that the address field refers to a register rather than a main memory address, basically the operand of the instruction is in the register specified:


Register Indirect Mode:
You point to a register, and the address you look for is within that register. Is like indirect addressing but instead of pointing to a word in memory, you point to a register.

Relativa o displacement:
Displacement addressing requires that the instruction have two address fields, at least one of which is explicit. The value contained in one address field (value = A) is used directly. The other address field, or an implicit reference based on opcode, refers to a register whose contents are added to A to produce the effective address.
EA = A + (R)
If you have 5 in the register and 7 in the instruction, the address would be 12.
Por base o desplazamiento:
    La instrucción de dirección contendrá el desplazamiento que se sumará al registro base previamente asignado
Por referencia al programa:
    El registro base en este caso es el contador de programa, que se sumará al desplazamiento dado por instrucción
Por paginación o yuxtaposición:
    Se divide la memoria de tal forma que pueda segmentarla en distintas páginas, por lo tanto para cada programa tendré distintas páginas. Cada que quiera direccionar solamente deberé hacer referencia a la página y el desplazamiento en base a esa página (5,10 sería página 5 posición 10 en base a esa página)


Indexado
Sirve para acceder a elementos dentro de un arreglo. Se suma a un número base pasado por instrucción, valores que aumentan de forma constante. Entras en el número de memoria 100, y vas aumentando 8 bits (byte), de forma constante, de esa manera puedes acceder a cada palabra dentro del arreglo.

Memorias
Things to take into account:

Faster access time, greater cost per bit;
Greater capacity, smaller cost per bit;
Greater capacity, slower access time.
1. Memory: In computer architecture, memory refers to the physical devices used to store data and instructions for processing by the CPU (Central Processing Unit) and other components of the computer. It is essential for the computer to function because it holds the programs and data that are currently being used.
2. Bits and Bytes:
    Bit: Short for binary digit, a bit is the smallest unit of data in a computer. It can hold one of two values: 0 or 1. It represents the most fundamental piece of information in computing.
    Byte: A byte is a group of 8 bits. Bytes are the basic units of storage in computer memory. They are used to represent characters, numbers, and other data types. For example, the letter 'A' might be represented by the byte 01000001.
3. Memory Units:
    Kilobyte (KB): Approximately 1,024 bytes.
    Megabyte (MB): Approximately 1,024 KB or 1,048,576 bytes.
    Gigabyte (GB): Approximately 1,024 MB or 1,073,741,824 bytes.
    Terabyte (TB): Approximately 1,024 GB or 1,099,511,627,776 bytes.
    Petabyte (PB): Approximately 1,024 TB or 1,125,899,906,842,624 bytes.
    Exabyte (EB): Approximately 1,024 PB or 1,152,921,504,606,846,976 bytes.
4. Memory Types:
    RAM (Random Access Memory): RAM is volatile memory used by the computer to store data that is being actively used or processed. It allows for quick access to data by the CPU. However, its contents are lost when the computer is turned off.
    ROM (Read-Only Memory): ROM is non-volatile memory that retains its contents even when the computer is powered off. It typically contains firmware or low-level software instructions that are essential for booting up the computer and initializing hardware.
    Cache Memory: Cache memory is a small, high-speed memory located between the CPU and main memory (RAM). It stores frequently accessed data and instructions to reduce the time it takes for the CPU to access them.
    Virtual Memory: Virtual memory is a memory management technique that uses a portion of the computer's hard drive as an extension of RAM. It allows the computer to run programs that require more memory than is physically available.
Understanding memory, bits, and bytes is fundamental to understanding how computers store and process information. These concepts form the basis of computer architecture and are essential for both hardware and software development.
Palabra
No hay una definición universal del término palabra. En general, una palabra es un conjunto ordenado de bytes o bits que es la unidad normal con la que se almacena, transmite, u opera la información dentro de un determinado computador. Normalmente, si un computador tiene un juego de instrucciones de longitud fija, la longitud de las instrucciones es igual a la de la palabra.
1. Word:
    In computer architecture, a word is the natural unit of data used by a particular processor design. It represents the maximum size of data that the CPU can process in one operation.
    The size of a word can vary depending on the architecture of the processor. Common word sizes include 8, 16, 32, and 64 bits. For example, in a 32-bit architecture, the word size is 32 bits, and in a 64-bit architecture, the word size is 64 bits.
    The size of a word often determines the maximum amount of memory that the processor can address directly. For instance, a 32-bit processor can address up to 2^32 (approximately 4.3 billion) memory locations.
2. Addressable Unit:
    The addressable unit is the smallest unit of memory that can be individually accessed or addressed by the CPU.
    In most modern computer architectures, the smallest addressable unit is typically a byte. This means that each memory location in the computer's memory is assigned a unique address, and each address corresponds to a byte of data. This is explained later with multiplexers
    For example, if a computer has 4 GB (gigabytes) of RAM and uses byte-addressable memory, it means there are approximately 4 billion memory locations, each corresponding to one byte of data.
So, to summarize, a word is the natural unit of data used by the CPU for processing, while a byte is the smallest addressable unit of memory, with each memory location in the computer's memory being uniquely identified by its address.

Design Constraints on Memory:
    Three fundamental questions: How much? How fast? How expensive?
How Much:
    Capacity is essential; applications will adapt to available capacity.
How Fast:
    Memory must keep pace with the processor to avoid performance bottlenecks.
How Expensive:
    Memory cost must be reasonable compared to other system components.
Trade-offs in Memory Design:
    Capacity, access time, and cost are interconnected.
Relationships Across Memory Technologies:
    Faster access time comes with a higher cost per bit.
    Greater capacity often correlates with a smaller cost per bit.
    However, greater capacity tends to lead to slower access times.
Design Dilemma:
    Balance between needing large-capacity, low-cost memory and high-performance, expensive, low-capacity memory.
Solution: Memory Hierarchy:
    Employing a hierarchy of memory types.
Memory Hierarchy:
    Smaller, expensive, faster memories at the top; larger, cheaper, slower memories at the bottom.
Hierarchy Characteristics:
    Decreasing cost per bit.
    Increasing capacity.
    Increasing access time.
    Decreasing frequency of access by the processor.
Explanation:
The text outlines the core considerations in memory design: capacity, access time, and cost.
It discusses trade-offs among these factors and the necessity of a memory hierarchy to balance performance and cost effectively.
The hierarchy ensures that the system has access to both fast, expensive memory for performance-critical tasks and larger, cheaper memory for storing larger amounts of data.
https://remnote-user-data.s3.amazonaws.com/htEXn0im5e8JWW4y2IgCHiyx2uEWuKNriXaSTtQePooprRLwXphgGZUlzw5-01-FIQnvdW2zR2poZ1RWoYadPUjsVvhBRq3VUid-2UQT7hcjwVRcUiqVpyEUtCkGFl_f.png
https://remnote-user-data.s3.amazonaws.com/BTFYjNKmgvUs6OU44QHkwuO7_t8JVeaUmHkvyXkdHKVW-gaxbRMYN8Xs89zlPsMdOAM245ga5C_RhlcSFhgPRvHyptWxRmVQDWrhsXwZbdfxGYyeN980FzouB5EtDfY7.png
1. Registers
Registers are small, high-speed memory units located in the CPU. They are used to store the most frequently used data and instructions. Registers have the fastest access time and the smallest storage capacity, typically ranging from 16 to 64 bits.
2. Cache Memory
Cache memory is a small, fast memory unit located close to the CPU. It stores frequently used data and instructions that have been recently accessed from the main memory. Cache memory is designed to minimize the time it takes to access data by providing the CPU with quick access to frequently used data.
3. Main Memory
Main memory, also known as RAM (Random Access Memory), is the primary memory of a computer system. It has a larger storage capacity than cache memory, but it is slower. Main memory is used to store data and instructions that are currently in use by the CPU.
Types of Main Memory
Static RAM: Static RAM stores the binary information in flip flops and information remains valid until power is supplied. It has a faster access time and is used in implementing cache memory.
Dynamic RAM: It stores the binary information as a charge on the capacitor. It requires refreshing circuitry to maintain the charge on the capacitors after a few milliseconds. It contains more memory cells per unit area as compared to SRAM.

4. Secondary Storage
Secondary storage, such as hard disk drives (HDD) and solid-state drives (SSD), is a non-volatile memory unit that has a larger storage capacity than main memory. It is used to store data and instructions that are not currently in use by the CPU. Secondary storage has the slowest access time and is typically the least expensive type of memory in the memory hierarchy.
5. Magnetic Disk
Magnetic Disks are simply circular plates that are fabricated with either a metal or a plastic or a magnetized material. The Magnetic disks work at a high speed inside the computer and these are frequently used.
6. Magnetic Tape
Magnetic Tape is simply a magnetic recording device that is covered with a plastic film. It is generally used for the backup of data. In the case of a magnetic tape, the access time for a computer is a little slower and therefore, it requires some amount of time for accessing the strip.
https://remnote-user-data.s3.amazonaws.com/2WIyZlDXGXRSzIcKxn-MFmMtW9X0nCahwRA5Yuh1BhITE7aRu2h4SM71I_JDSMubL4Jr6QFNFK-Q6tAgAk61Uophmp9mVckuKvYTuKHH7zkdq4V5Pt-jGBviZiFjNCuK.png


Entrada y Salida
Input/Output (I/O): This section introduces the concept of Input/Output in computer systems, emphasizing its importance in facilitating communication between the computer and external devices. It discusses the role of I/O in enabling users to interact with computers and for computers to communicate with peripherals like keyboards, mice, printers, and storage devices.
What is an I/O module?
An I/O (Input/Output) module is a component within a computer system responsible for managing communication between the CPU (central processing unit) and peripheral devices. It serves as an interface that enables the CPU to interact with external devices such as keyboards, mice, monitors, printers, storage devices, and network adapters. The I/O module contains logic circuits that facilitate data transfer between the CPU and peripherals, translating commands from the CPU into signals that can be understood by the connected devices, and vice versa. Additionally, I/O modules often provide buffering and error-handling mechanisms to ensure reliable data transmission between the CPU and peripherals. Overall, I/O modules play a crucial role in enabling the computer system to interact with its external environment, facilitating input and output operations essential for performing tasks and running applications.
https://remnote-user-data.s3.amazonaws.com/QgmuNfw-cGqq_iIhrXzTIAUDVXwIwudzBPwEHjS8a4tcblB03UDeICtACNFaEwOL8kxbe5aTsvbFEERSzCHPDFGvWVZBIAXMGQoSRejcAkZvUOR4nhQqZI1RnIdhaQWY.png

Overview of I/O Operations:  
    In a computer system, I/O operations involve using various external devices to exchange data between the computer and the external environment.
    These external devices connect to the computer via links to I/O modules, facilitating the exchange of control signals, status updates, and data.
    External devices connected to I/O modules are commonly referred to as peripheral devices or peripherals.
    
External Devices: 
Here, various types of external devices are explored, ranging from simple devices like keyboards and mice to more complex peripherals such as printers, scanners, and storage devices like hard drives and solid-state drives (SSDs). The section may also discuss the characteristics and interfaces of different external devices.

Classification of External Devices:  
External devices can be broadly categorized into three types:
    1. Human Readable: Devices designed for communication with the computer user, such as monitors, keyboards, and touchscreens.
        These devices are designed for humans to interact with the computer, like video display terminals (VDTs) and printers. They display information in a format that people can easily understand.
    2. Machine Readable: Devices intended for communication with equipment, such as barcode scanners, sensors, and actuators.
        These devices are meant to communicate with other machines or equipment. Examples include magnetic disk and tape systems, as well as sensors and actuators used in robotics. They usually process data in a format that's suitable for machines.
    3. Communication: Devices suitable for communicating with remote devices, such as modems, network adapters, and wireless transceivers.
        These devices facilitate communication between the computer and remote devices. They enable data exchange over long distances. Examples could be modems or network adapters.

In simple terms, input/output (I/O) operations involve using various external devices to exchange data between a computer and the outside world. These devices connect to the computer through an I/O module, which serves as the link for transferring control signals, status updates, and actual data between the device and the computer.
For instance, when you type on a keyboard, the keyboard is a human-readable device. The data you input is sent to the computer through the I/O module. Similarly, when a computer sends a print job to a printer, the printer is a human-readable device, and the data is sent through the I/O module.
It's important to note that while devices like disk and tape systems are often considered part of the computer's memory hierarchy, they are controlled by I/O modules for data transfer, which is why they are discussed in this chapter focusing on I/O operations.
When a computer wants to use a device, it sends control signals to tell the device what to do, like sending data or receiving it. The device then does its job with the help of control logic. For example, a disk drive might move its reading head to a specific position based on instructions from the computer.
Data is sent between the device and the computer in the form of bits (0s and 1s), and the device might need to convert this electrical data into other types of energy (like sound or movement) or vice versa.
To manage this data transfer smoothly, there's usually a buffer associated with the device. This buffer temporarily holds data as it moves between the device and the computer. Buffers can vary in size depending on the type of device. For instance, simple devices like keyboards might have small buffers, while complex ones like disk drives might have much larger ones.

Useful definitions
    1. Communication devices: These are devices that enable a computer to send and receive data to and from other devices, which could be anything from a keyboard or a printer to another computer.
    2. Control signals: These signals determine what action a device will perform, like sending data to the computer (INPUT or READ), receiving data from the computer (OUTPUT or WRITE), indicating its current status, or performing specific functions (like positioning a disk head in a disk drive).
    3. Data signals: This refers to the actual information being sent to or received from the computer, usually in the form of binary digits (bits).
    4. Status signals: These signals indicate the current state of the device, such as whether it's ready to transfer data or not.
    5. Control logic: This is the part of the device that controls its operation based on instructions received from the computer. It ensures that the device performs the necessary tasks according to the commands it receives.
    6. Transducer: This component converts data between different forms of energy, for example, converting electrical signals to physical movement (like positioning a disk head) or vice versa.
    7. Buffer: A buffer is a temporary storage area that holds data being transferred between the device and the computer. It helps manage the flow of data, especially when there might be differences in speed between the two.
    8. Interface: This is the connection point between the device and the computer, allowing them to communicate with each other.
    
    
Keyboard Example  
The most common way for users to interact with computers is through a keyboard and monitor setup.
Users input data through the keyboard, which is then transmitted to the computer and may also be displayed on the monitor.
The monitor also displays data provided by the computer.
Characters are the basic units of exchange, each associated with a code typically 7 or 8 bits long, with the International Reference Alphabet (IRA) being a commonly used text code.
IRA uses 7-bit binary codes, allowing for the representation of 128 different characters.
Characters are classified into printable and control characters, with printable characters being those that can be printed or displayed on a screen, and control characters used for controlling printing/displaying or communications procedures.
When a key is pressed on the keyboard, it generates an electronic signal interpreted by the keyboard's transducer and translated into the corresponding IRA code bit pattern.
This pattern is then transmitted to the computer's I/O module for processing and storage.
On output, IRA code characters are transmitted from the computer to external devices via the I/O module.
The transducer at the device interprets the code and sends the necessary electronic signals to display the character or perform the requested control function.
https://remnote-user-data.s3.amazonaws.com/WFFB2o896B7QuoE690Acc74BLmWVkda7UtKVrbFpmnunzZ4PFMh4sXmNp9IQDPygBG78B1xh9ylWB4kkOSeVh_omWq-rEur3UdEq53krOi9Li_6wYHxGZ5z9rpuv5Mz1.png





I/O Modules:
This section covers the hardware components responsible for managing I/O operations, known as I/O modules. It explains their role in controlling data transfer between the CPU and external devices, including handling data formatting, error detection, and device control.
The major functions or requirements for an I/O module fall into the following categories:
Control and timing
Processor communication
Device communication
Data buffering
Error detection
During any period of time, the processor may communicate with one or more external devices in unpredictable patterns, depending on the program’s need for I/O. The internal resources, such as main memory and the system bus, must be shared among a number of activities, including data I/O. Thus, the I/O function includes a control and timing requirement, to coordinate the flow of traffic between internal resources and external devices. For example, the control of the transfer of data from an external device to the processor might involve the following sequence of steps:
The processor interrogates the I/O module to check the status of the attached device.
The I/O module returns the device status.
If the device is operational and ready to transmit, the processor requests the transfer of data, by means of a command to the I/O module.
The I/O module obtains a unit of data (e.g., 8 or 16 bits) from the external device.
The data are transferred from the I/O module to the processor.
The I/O module plays a crucial role in communication between the processor and external devices. Processor communication involves:
Command decoding: Commands from the processor are interpreted by the I/O module, often transmitted via the control bus. For instance, commands for a disk drive might include operations like READ SECTOR or WRITE SECTOR, each possibly carrying parameters sent over the data bus.
Data exchange: Data moves between the processor and the I/O module via the data bus.
Status reporting: Given the slow nature of peripherals, it's essential to track the I/O module's status. Signals like BUSY and READY inform the processor about the module's readiness or ongoing tasks, alongside signals for error conditions.
Address recognition: Similar to memory addressing, each I/O device possesses a unique address. Thus, the I/O module must identify and respond to the address corresponding to each peripheral it manages.

I/O Module Structure  
https://remnote-user-data.s3.amazonaws.com/iE-Y5BUq4OM9RvMASJQBPVfgH8o6aV6gWm7rIDTL_xpePW7CbJbqW8-V21ZcQGRGjHfAD-lai77E8JmoMhd3oufEjzSXb9h7o_iyRWMQGm8wCKTId-OI5pIyF6dGz8V5.png


I/O techniques
Programmed I/O (PIO)
Direct Memory Access (DMA):
Interrupt-Driven I/O:

Programmed I/O: 
When the processor executes a program and encounters an instruction related to I/O, it issues a command to the appropriate I/O module. With programmed I/O, the module performs the requested action and sets the corresponding bits in the I/O status register. However, it does not further engage with the processor, including interrupting it. Thus, the processor must periodically check the module's status until the operation is complete.
The image that compares the 3 methods provides an example of using programmed I/O to read a block of data from a peripheral device (such as a record from tape) into memory. Data are read one word (e.g., 16 bits) at a time. For each word read, the processor must remain in a status-checking cycle until it confirms that the word is available in the I/O module's data register. This flowchart illustrates the primary drawback of this technique: it's a time-consuming process that needlessly occupies the processor.


I/O commands  
To execute an I/O-related instruction, the processor issues an address specifying the particular I/O module and external device, along with an I/O command. There are four types of I/O commands that an I/O module may receive when addressed by a processor:
Control: Used to activate a peripheral and define its action. For instance, a magnetic tape unit may be instructed to rewind or advance one record. These commands are customized for specific types of peripheral devices.
Test: Employed to check various status conditions associated with an I/O module and its peripherals. The processor ensures that the peripheral is powered on and available for operation. It also verifies if the most recent I/O operation is complete and if any errors occurred.
Read: Initiates the I/O module to retrieve data from the peripheral and store it in an internal buffer (depicted as a data register in Figure 7.3). The processor can then access the data by requesting the I/O module to place it on the data bus.
Write: Instructs the I/O module to receive data (byte or word) from the data bus and transmit it to the peripheral.

https://remnote-user-data.s3.amazonaws.com/TI_Df9pA9ruYcnJTZsT2fbZQla5Ogt4k0-wKuFyBqemKrYM7DtFL4Atz25GH0kOhDgT6UhpiBYWeyr4YSWkCIttbTaxXxEeSwa_Ti-c6yMwe-87YRyz74hUONMzRyOWT.png

1. Programmed I/O (PIO):
Programmed I/O is the most basic form of I/O handling. In this method, the CPU is directly responsible for transferring data between the I/O device and memory. The CPU executes specific instructions to read or write data to/from the I/O device. It involves the CPU checking the status of the I/O device, issuing commands to it, and then transferring data between memory and the device.
Advantages:
    Simple implementation.
    Suitable for transferring small amounts of data or when the frequency of I/O operations is low.
Disadvantages:
    Inefficient for transferring large amounts of data due to the high overhead on the CPU.
    CPU is tied up during I/O operations, reducing overall system performance.
2. Direct Memory Access (DMA):
DMA is a method that allows data to be transferred directly between an I/O device and memory without involving the CPU. DMA controllers are specialized hardware units that manage these data transfers. The CPU sets up the DMA controller with information about the data transfer (source, destination, size, etc.), and then the DMA controller takes over the data movement while the CPU is free to perform other tasks.
Advantages:
    Offloads data transfer tasks from the CPU, improving overall system performance.
    Particularly effective for transferring large amounts of data.
Disadvantages:
    Requires additional hardware (DMA controller).
    More complex to implement than programmed I/O.
3. Interrupt-Driven I/O:
In interrupt-driven I/O, the CPU is not constantly polling the I/O device to check if it needs attention. Instead, the CPU initiates an I/O operation and then continues executing other tasks. When the I/O device needs attention (e.g., data is ready for transfer or an operation is complete), it interrupts the CPU, causing it to temporarily suspend its current task and handle the I/O request.
Advantages:
    Allows the CPU to perform other tasks while waiting for I/O operations to complete.
    Improves overall system responsiveness.
Disadvantages:
    Requires hardware support for interrupt handling.
    More complex to implement than programmed I/O.
In summary, programmed I/O involves the CPU directly managing data transfers between memory and I/O devices, DMA offloads this task to a specialized controller to improve performance, and interrupt-driven I/O allows the CPU to multitask while handling I/O operations by responding to interrupts from devices. Each method has its advantages and is suited to different scenarios based on factors like data transfer size, frequency, and system performance requirements.

When to use which?
1. Programmed I/O (PIO):
Best for:
    Simple I/O operations with low data transfer rates and sporadic events.
Example Scenario:
    Reading input from a single button on a microcontroller-based device. The device only needs to check the status of the button occasionally, and the data transfer involves only a single bit. Using programmed I/O, the microcontroller can periodically check the state of the button by reading a specific memory address or I/O port associated with the button input.
2. Direct Memory Access (DMA):
Best for:
    Large data transfers with minimal CPU involvement.
Example Scenario:
    Transferring a large file from a hard disk drive to system memory in a computer. The CPU initiates the DMA transfer by providing the DMA controller with the source (disk) and destination (memory) addresses and the size of the data to be transferred. The DMA controller then handles the data transfer directly between the disk and memory, allowing the CPU to perform other tasks simultaneously without being tied up by the data transfer process.
3. Interrupt-Driven I/O:
Best for:
    Systems requiring prompt response to external events.
Example Scenario:
    Network communication in a server. When data packets arrive from the network interface card, they trigger interrupts, prompting the CPU to handle the incoming data immediately. This allows the system to respond quickly to incoming network requests without continuously polling the network interface.
Example with  keyboard and mouse
1. Keyboard:
    Keyboards generate input events (keystrokes) sporadically and intermittently.
    Each keystroke needs to be processed promptly to maintain smooth user interaction.
    Using interrupt-driven I/O, the keyboard can interrupt the CPU whenever a key is pressed or released, ensuring immediate processing of each keystroke without the need for constant polling by the CPU.
    This method allows the CPU to remain responsive to other tasks while still handling keyboard input efficiently.
2. Mouse:
    Similar to keyboards, mice also generate input events (movements and clicks) sporadically.
    Mouse input requires immediate response for accurate cursor movement and interaction with graphical elements.
    Interrupt-driven I/O allows the mouse to interrupt the CPU whenever movement or button clicks occur, ensuring that the mouse input is processed promptly and accurately.
    This method enables smooth and responsive cursor movement without requiring continuous CPU polling.
8. I/O Channels and Processors: I/O channels and processors are specialized units dedicated to handling I/O operations efficiently. This section discusses their architecture, functions, and how they collaborate with the CPU and other system components to manage I/O.
9. External Interconnection Standards: This part covers the standards and protocols used for connecting external devices to computers, such as USB, Thunderbolt, SATA, and Ethernet. It explains their features, compatibility, and typical usage scenarios.
10. IBM zEnterprise EC12 I/O Structure: This case study provides insights into the I/O architecture of the IBM zEnterprise EC12 mainframe system. It may discuss its unique features, scalability, and how it handles I/O operations in large-scale computing environments.
11. Key Terms, Review Questions, and Problems: This section summarizes the key terms introduced in the chapter, provides review questions to test understanding, and presents problems to reinforce concepts through practical application.




















Preguntas de la guía 1
1. ¿Qué es una computadora?
    Una computadora es un dispositivo electrónico diseñado para procesar datos de manera automática mediante la ejecución de programas. Sus componentes fundamentales son:
    CPU (Unidad Central de Procesamiento): Realiza las operaciones de cálculo y control en la computadora.
    Memoria principal: Almacena temporalmente datos e instrucciones que el CPU necesita para procesar.
    Dispositivos de entrada: Permiten al usuario ingresar datos a la computadora (como teclado, ratón, etc.).
    Dispositivos de salida: Muestran resultados o información procesada por la computadora (como pantalla, impresora, etc.).
    Dispositivos de almacenamiento: Guardan datos a largo plazo (como discos duros, unidades de estado sólido, etc.).
2. ¿Qué es el CPU?
    El CPU (Unidad Central de Procesamiento) es el componente principal de una computadora, encargado de ejecutar las instrucciones de los programas y realizar operaciones aritméticas y lógicas. Está compuesto por la unidad de control, que coordina las operaciones, y la unidad aritmético-lógica, que realiza cálculos y operaciones lógicas.
3. ¿A qué se llama memoria principal? ¿Cuál es su función? Ejemplifique.
    La memoria principal es un tipo de almacenamiento temporal de acceso rápido donde se almacenan datos y programas que están en uso activo por el CPU. Su función principal es proporcionar un espacio de trabajo para el procesador, permitiéndole acceder rápidamente a los datos que necesita para ejecutar instrucciones. Ejemplo: la RAM (Memoria de Acceso Aleatorio) es un tipo de memoria principal donde se cargan los programas y datos que se están utilizando en un momento dado.
4. ¿A qué se llama memoria secundaria? ¿Cuál es su función? Ejemplifique.
    La memoria secundaria es un tipo de almacenamiento de acceso más lento pero de mayor capacidad que la memoria principal. Su función principal es almacenar datos de manera permanente, incluso cuando la computadora está apagada. Ejemplo: los discos duros y las unidades de estado sólido (SSD) son tipos de memoria secundaria donde se almacenan archivos y programas de manera permanente.
5. ¿A qué se llama almacenamiento fuera de línea?
    El almacenamiento fuera de línea se refiere a cualquier forma de almacenamiento que no está directamente conectada o accesible para el sistema en un momento dado. Esto puede incluir dispositivos de almacenamiento como discos duros externos, unidades flash USB o incluso servicios en la nube a los que se accede a través de internet.
6. ¿Qué es una jerarquía de memorias?
    La jerarquía de memorias es un concepto que describe la organización de diferentes niveles de almacenamiento en una computadora, cada uno con diferentes velocidades de acceso y capacidades. En general, cuanto más cerca esté un nivel de memoria del CPU, más rápido será el acceso pero menor será su capacidad, y viceversa.
7. Defina el concepto de memoria caché.
    La memoria caché es un tipo de memoria de acceso rápido y tamaño reducido que se encuentra entre el CPU y la memoria principal en la jerarquía de memorias. Su función principal es almacenar temporalmente datos e instrucciones que el CPU necesita acceder con frecuencia, reduciendo así el tiempo de acceso a la memoria principal y mejorando el rendimiento del sistema. La memoria caché opera según el principio de la localidad de referencia, que establece que los programas tienden a acceder a los mismos datos o instrucciones repetidamente en un corto período de tiempo.
8. Defina el concepto de buffer:
    Un buffer es una región de memoria temporal utilizada para almacenar datos mientras se transfieren entre dos dispositivos o procesos con diferentes velocidades de operación. Funciona como un área de almacenamiento intermedio que permite una comunicación más eficiente entre los componentes que operan a diferentes velocidades. Por ejemplo, en la reproducción de audio o video en línea, un buffer puede almacenar fragmentos de datos anticipadamente para evitar interrupciones durante la reproducción cuando la conexión de red es lenta.
9. ¿Qué es la memoria virtual?
    La memoria virtual es una técnica que utiliza el sistema operativo para ampliar la capacidad de la memoria física de una computadora al permitir que partes de los programas y datos que no se están utilizando activamente se almacenen temporalmente en el disco duro. Esto permite que los programas utilicen más memoria de la que está físicamente disponible en la RAM. La memoria virtual se gestiona mediante un sistema de paginación o segmentación, donde se dividen los programas en fragmentos llamados páginas o segmentos, que se cargan y descargan según sea necesario.
10. ¿Cuáles son los componentes fundamentales del CPU?
    Los componentes fundamentales del CPU son:
    Unidad de Control (UC)
    Unidad Aritmético Lógica (ALU)
    Registros internos
11. ¿Cuál es la función de la UC (Unidad de Control)?
    La función principal de la Unidad de Control es interpretar y ejecutar las instrucciones del programa. Coordina las operaciones del CPU, controla el flujo de datos entre la CPU y otras partes del sistema, y se encarga de buscar, decodificar y ejecutar las instrucciones almacenadas en la memoria.
12. ¿Cuál es la función de la ALU (Unidad Aritmético Lógica)?
    La función principal de la ALU es realizar operaciones aritméticas (como sumas y restas) y operaciones lógicas (como AND, OR y NOT) sobre los datos que recibe del registro interno y de la memoria principal.
13. ¿Qué elemento de la UC me indica la dirección de la siguiente instrucción a ejecutarse?
    El Program Counter (Contador de Programa) es el elemento de la Unidad de Control que indica la dirección de la siguiente instrucción a ejecutarse. Es un registro que almacena la dirección de memoria de la siguiente instrucción que el CPU debe recuperar y ejecutar.
14. ¿Qué es el ciclo de vida de una instrucción y cuáles son sus fases?
    El ciclo de vida de una instrucción es el proceso que sigue una instrucción desde que se carga en el CPU hasta que se completa su ejecución. Sus fases son:
    Buscar: El CPU busca la siguiente instrucción en la memoria.
    Decodificar: La Unidad de Control interpreta la instrucción y determina qué acción realizar.
    Ejecutar: La instrucción se ejecuta, lo que puede implicar operaciones aritméticas, lógicas o de transferencia de datos.
    Almacenar (si es necesario): Algunas instrucciones pueden requerir almacenar resultados en la memoria o en registros específicos.
15. Explique qué son las técnicas de direccionamiento. Explique y distinga los modos directo, indirecto, inmediato y por base y desplazamiento.
    Las técnicas de direccionamiento se refieren a los métodos utilizados para especificar la dirección de los operandos en una instrucción de máquina. Los modos comunes son:
    Directo: La dirección del operando se especifica directamente en la instrucción.
    Indirecto: La instrucción contiene la dirección de memoria donde se encuentra la dirección del operando.
    Inmediato: El operando en sí mismo se especifica directamente en la instrucción.
    Por base y desplazamiento: Se suman una dirección base almacenada en un registro y un desplazamiento especificado en la instrucción para calcular la dirección del operando.
16. ¿Qué son los periféricos?
    Los periféricos son dispositivos conectados a una computadora que proporcionan funcionalidades adicionales para realizar tareas específicas de entrada, salida o almacenamiento de datos. Ejemplos comunes incluyen teclados, ratones, impresoras, escáneres, discos duros externos, etc.
17. Explique los mecanismos para tratamiento de E/S: Guiado por programa, por interrupciones y acceso directo a memoria.
    Guiado por programa: El CPU controla directamente el flujo de datos de entrada y salida entre la memoria y los periféricos. Este enfoque requiere una cooperación explícita del programa para realizar operaciones de E/S.
    Por interrupciones: Los periféricos pueden interrumpir el flujo normal de ejecución del CPU para señalar que necesitan atención. El CPU responde a estas interrupciones ejecutando rutinas de servicio de interrupción para manejar las operaciones de E/S.
    Acceso directo a memoria (DMA): Los periféricos con capacidades DMA pueden transferir datos directamente entre sí y la memoria principal sin intervención del CPU, lo que libera al CPU para realizar otras tareas mientras se lleva a cabo la transferencia de datos.
