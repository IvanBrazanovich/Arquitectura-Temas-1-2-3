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
    - 
