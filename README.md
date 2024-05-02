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
<html>
  <head>
    <style>
      .Portal {
        border-color: lightblue;
        border-style: solid;
      }
    </style>
  </head>
  <body>
    <h1>
      Tema 1: Fundamentos de arquitecturas de computadoras mejorado
    </h1>
    <br/>
    <ul>
        <li>Guías y temas</li>
        <li><u><b>Videos:</b></u></li>
        <li>Crash course for the first part</li>
        <li><a isInlineLink="true" href="https://youtu.be/n31IHq2FnN8?feature=shared">https://youtu.be/n31IHq2FnN8?feature=shared</a> (Arquitectura VN)</li>
        <li><a isInlineLink="true" href="https://youtu.be/ii4-MCNE0zs?feature=shared">https://youtu.be/ii4-MCNE0zs?feature=shared</a> (Direccionamientos parte 1)</li>
        <li><a isInlineLink="true" href="https://youtu.be/y4Lnl6B7Sxo?feature=shared">https://youtu.be/y4Lnl6B7Sxo?feature=shared</a> (Direccionamiento parte 2)</li>
        <li><a isInlineLink="true" href="https://youtu.be/aUB80lCfnyA?feature=shared">https://youtu.be/aUB80lCfnyA?feature=shared</a> (Memorias)</li>
        <li><a isRemReference="true" href="https://youtu.be/fvXi6mNFXwo?isPin=false">Subrutinas - YouTube</a> subrutinas</li>
        <li></li>
        <li><u><b>Temas: </b></u> La Computadora, Arquitectura de Von Neumann. Microprocesadores, subrutinas y lenguajes de bajo nivel . Técnicas de Direccionamientos . Memorias . Entrada y Salida. Subrutinas.</li>
        <li>How are the basics of a computer built? </li>
        <li><u><b>Note</b></u> </li>
        <li>Almost everything here is built with logic gates, CPU, Control unit, ALU, RAM, etc.  They look like this:
<img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F4OeCqQT_EeSQ_jMDz2c-d4UDvUSSowcr38ppQXpC7z6bhOR4goEB-YSoQZedkBP1bBCGUbER1RvJUw3OmH28vw9ftlpe7NqSXHvW4Ci9YO3q1P3WMy_Z1a6uZcENVAOi.png" width="790" height="597.4375"/></li>
        <li></li>
        <li>How do transistors work?   </li>
        <li>In the context of computers, transistors work like a switch (on/off). A transistor can act as a switch or gate for electronic signals, opening and closing an electronic gate many times per second. It ensures the circuit is on if the current is flowing and switched off if it isn&#39;t.</li>
        <li>If you turn on the b wire, you allow current to flow in the c-e section.</li>
        <li>The b wire is called a control wire</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FC7o-5sjHu0ra-79qlYsxBU2VDpp9LVY_vRXq3g41pJBkyxXWzZvs-1uiiTgG-KNYHuZjryuAzEy5EnnwFAg7ka9Bi0digC-ToU9_Wuw_kP2XWNkAtSccFENGnCoVXsqG.png" width="183" height="193"/></li>
        <li></li>
        <li>Basically sillicon is an element that is semiconductor, but if you apply doping to it (adding other elements with different structures) you can increase the amount of electrons in the material or decrease it, making it easier for electrons to flow and form a current.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fy4nR5hkTj_jhIX9ZqODMXFQh_5hNE1BvqNdZBN6EKAqWiHdbh0XsNj0xKGNm_JliCnhBXwqDqsj0Ru48HsxXokZ0HuYS50TlM2mGysMncrOo4A0tmM6Dw6qAw-thi36s.png" width="790" height="342.6625"/></li>
        <li>In this case you have n-type and p-type doped sillicon. P-type is has more &quot;holes&quot; that could be filled with electrons, and n-type has more electrons. As soon as the materials get together, the electrons on the more negative side feel attracted to the positive holes and they move towards them. This movement creates a zone called &quot;región de agotamiento&quot; que crea una barrera que previene el flujo de corriente.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FELFAxCoXdWbiD9BNtXL0NtiPPgFXX2jpaR9dgO0zxKKaLxbeBKe-7_xjcrpR0STJxo9DGsd6Vvf8I4WxMZOFPOxgXf_NwHMxPyM26URhH0uob4S3695WphTAYvLNWirn.png" width="790" height="342.6625"/></li>
        <li>However, if you apply a positive voltage to the base, the electrons in the material flow towards it, reducing the repulsion that the depletion layer had and allowing a flow of current to go through it.</li>
        <li><u><i>Step 1:</i></u> </li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fdo9uGUhBgMSPUyHa_t74VC47SP1bdofAMMJxsCABFsM5eXHRzpLzedxQmrObZOfpZEJkuF4n0RdbktuGY0tScdvR8jdHL8h9-Ywvnv8jHQ1vXeDUOez1TzWSwd7-rQwN.png" width="790" height="480.9125"/></li>
        <li><u><i>Step 2:</i></u> </li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Ff4MDatBfFJcu27XyD-WnFKXfiEK6uryPQaFydjt9JzCqNtXhrREk4etmbaiCwxxmcQAPPBXeUCgW4_n9DqGZDoR2FZQJWRQSv8p1DLwXLXgKMkwZXbdOeDCK9JAhvNZS.png" width="790" height="480.9125"/></li>
        <li></li>
        <li></li>
        <li><b>Boolean algebra and logic gates</b></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FTaQI8gbdtdfoUFplWrUyeQv6OlVtRo1ZlEX9gYTp3xKjNGRR_sl_TLmW4gvzMT2azU9Wyjl-MiDPfIm5M2k-erWW8xLnmEU8ExWopNAJ0tzs3aBu6VwuqTXx2-NTY3Zo.png" width="790" height="279.46250000000003"/></li>
        <li></li>
        <li>We can build boolean algebra with transistors.</li>
        <li>You can consider the control wire as input and the bottom wire as output. When the control wire (or input) is on, then the output is 1, when the input is off, the ouput is 0.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F4lkk8dlO7I2SmzjUtSGHviMwbIfenIUdRayyqJtmYclaAy6WK29fWpuXYRDab7Lv63L2SYp1ELYZWLzAo6ugSUWAd-PY42WN_XNqCSAzEoFO5FIAcmvF6MxFN8yphjnw.png" width="444" height="438"/></li>
        <li></li>
        <li></li>
        <li><u><b>Not gate</b></u> </li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FxUpbWC70XQUMPaxwx4BYGMFknMCtM7kRcGJv57sb1iOhM6K8cyd6fg-FJvk7zH9hmzHgTYrOATojv8A6lheP9_wGkZ2DjRQRtL-pw93GisqZP6Wq2n4yyXG8kKW7KmVo.png" width="278" height="170"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FOB2Ohu3ZTgcFq-2YTKJoGRL3QsijTzU3mOT-GDkfUI-RupWswN_UxL1VOW6Ll9qCpaZjHP8Olm1GuR6_cEJB_9rLeUlh4wtEr1ZeSBG6SMNZssA7weCh542SPCEuskLB.png" width="790" height="489.8"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F6pf4httHlvlZ9UZGdeaHjDfatYsd1l3V2scStVWNNDal4OiiVOpAWNtFqUJdzqeSsuYD2-A3OQ4z4khhHo4fnJ6m2VckbwPMTimJvg_9k9hdXcFZTNxk0O2Qbux7N2xb.png" width="790" height="489.8"/></li>
        <li></li>
        <li></li>
        <li></li>
        <li><u><b>And gate</b></u> </li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fboozw1wBgyjRv9RbdpHopF5fi8JP7JU30hZueCxcbHXmiHtemoFvjmeSk1957yPyV26DfAtSk3nL2zHu5-DXLYxVxj6W2N_MzGN2QQnyuuBTEMrXzDEOLUVEY7-QDdQQ.png" width="747" height="433"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F0X8LrE84p5wWHcmA07AthsvRkXds8CF4_JL5GrvgrehN0sGb97OnCJSucCBQXhRatRHhvbtnh-uqY16sedazjGOcd6ldWp3Dgm_kdqzHiafsl-wfHOA1rPGJteVcLN-1.png" width="790" height="415.7375"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fg5rWgDnnC4-hQHxCiAT5UQR8EpCgpEJKdaSNtmWEt0Cce0N6D9BDQyHm0LElDGwy9EoQ-btWhArhLASRjch-JogWzSb29R8jC9Eq9J_CnvBEsKCq9xFwyGghwpTaBYR2.png" width="790" height="415.7375"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FEAH74Nu5KnyF-jkNj1hBO5Lxx3dN1aj34sivpbN2ONifODTLKjJNzdegQ9IF6mQsvlQ3rKPJ1ZrweFoMEj9a3aGlOFanz_bDTg4NJhicfFo0iJb_JdBNHjKB9hGqL6ol.png" width="790" height="415.7375"/></li>
        <li></li>
        <li></li>
        <li></li>
        <li><u><b>OR gate</b></u> </li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fs9ACvzvmcfQ5dLrA6n-IEgrnYJU0C36ZxiyTd1ADqDWu4-gF7nUMCNzJGt6c0_4ohj1sLz1EcryRHaU814arTxRLTNpuvXLICoyCr9fh4ChJ4vPpVzYY3qiDxBBc6kLx.png" width="628" height="367"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FkhTCNVeRSFesD6zyJpegbVtqbIqfAipCNyAUl1iirRCsTfkYiVefRTcjkgnKZf9Z-qoKw7-Z25EjTPWryJf6qjvZRY53nKBwLPAKvrI3LFXe3cLe_x3aIIMjWd-rExR3.png" width="790" height="415.7375"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FEHSfkn67wu9C3P6tjx0lNLM1JiHduKn6thdiPGW0KXorGkv4m13-t87WmNWPngl9LM3qW4z7froIcJxfutkYn-RPE0O9YzLRusYfOb3-_KdJkjhZ-NH0jVn87nZ05r6S.png" width="790" height="415.7375"/></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li><u><b>Exclusive OR  (XOR)</b></u> </li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fg9ldKfpqe7J1cjV8nTLjsHjfcNEcqPKHPla4_7A_i3N27lLfwB3iHf1556f9b5OzeaUVwu0jLGvGw05iG1-TB_Fl30EdebEjRwjOWNYioRQM4JqR91FyxpbJ4zgi3h-3.png" width="628" height="367"/></li>
        <li><u><b>photo of xor (I will save them in whatsapp )</b></u></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li><b>Representing numbers and letters with binary</b></li>
        <li></li>
        <li>In base 10, you have 10 numbers to work with (0-9), however, if you stack them up you can represent more information than the basic 9 numbers, the same happens with binary.</li>
        <li>For example, 256 is just (2x10^2 + 5 x10^1 + 6x10^0 ).</li>
        <li>In base two notation, instead of having multipliers of 10, you only have 2 numbers you can use to represent, which means you have multipliers of 2 (1, 2, 4, 8, 16, ...  2^n) instead of (1, 10, 100, ... 10^n)</li>
        <li>1. <b>Base-2 Notation (Binary)</b>:
            <ul>
                <li>In base-2 notation, also known as binary, each digit&#39;s position represents a power of 2. The rightmost digit represents $2^0$, the next digit to the left represents $2^1$, then $2^2$, and so on.</li>
            </ul>
        </li>
        <li>2. <b>Possible Digits</b>:
            <ul>
                <li>In binary, there are only two possible digits: 0 and 1. This means that each digit in a binary number can only be one of these two digits.</li>
            </ul>
        </li>
        <li>3. <b>Possible Combinations</b>:
            <ul>
                <li>The number of possible combinations of digits within a binary number of length n is determined by the base (2). Since each position can be either 0 or 1, there are 2 possibilities for each position. Therefore, the total number of possible combinations for an n-digit binary number is $2^n$.</li>
                <li>For example:</li>
                <li>For a single-digit binary number (n = 1), there are $2^1 = 2$ possible combinations: 0 and 1.</li>
                <li>For a two-digit binary number (n = 2), there are $2^2 = 4$ possible combinations: 00, 01, 10, and 11.</li>
                <li>For a three-digit binary number (n = 3), there are $2^3 = 8$ possible combinations: 000, 001, 010, 011, 100, 101, 110, and 111.</li>
                <li>And so on.</li>
            </ul>
        </li>
        <li>4. <b>Example</b>: Let&#39;s consider a 4-digit binary number. The possible combinations are:</li>
        <li>0000</li>
        <li>0001</li>
        <li>0010</li>
        <li>0011</li>
        <li>0100</li>
        <li>0101</li>
        <li>0110</li>
        <li>0111</li>
        <li>1000</li>
        <li>1001</li>
        <li>1010</li>
        <li>1011</li>
        <li>1100</li>
        <li>1101</li>
        <li>1110</li>
        <li>1111</li>
        <li>In summary, base-2 (binary) notation consists of two possible digits (0 and 1), and the number of possible combinations for an n-digit binary number is $2^n$. This makes binary notation essential for digital systems and provides a foundation for understanding and working with computers and digital electronics.</li>
        <li></li>
        <li>In base-10 notation (decimal), each digit&#39;s position represents a power of 10. The rightmost digit represents $10^0$, the next digit to the left represents $10^1$, then $10^2$, and so on.</li>
        <li></li>
        <li>1. <b>Possible Digits</b>:
            <ul>
                <li>In base-10, there are ten possible digits: 0, 1, 2, 3, 4, 5, 6, 7, 8, and 9. Each digit in a decimal number can be one of these ten digits</li>
            </ul>
        </li>
        <li>2. <b>Possible Combinations</b>:
            <ul>
                <li>The number of possible combinations of digits within a decimal number of length n is determined by the base (10). Since each position can be any of the ten digits, there are 10 possibilities for each position. Therefore, the total number of possible combinations for an n-digit decimal number is $10^n$.</li>
                <li>For example:</li>
                <li>For a single-digit decimal number (n = 1), there are $10^1 = 10$ possible combinations: 0, 1, 2, 3, 4, 5, 6, 7, 8, and 9.</li>
                <li>For a two-digit decimal number (n = 2), there are $10^2 = 100$ possible combinations: 00, 01, 02, ..., 99.</li>
                <li>For a three-digit decimal number (n = 3), there are $10^3 = 1000$ possible combinations: 000, 001, 002, ..., 999.</li>
                <li>And so on.</li>
            </ul>
        </li>
        <li>3. <b>Example</b>: Let&#39;s consider a 3-digit decimal number. The possible combinations are:
            <ul>
                <li>000</li>
                <li>001</li>
                <li>002</li>
                <li>...</li>
                <li>998</li>
                <li>999</li>
            </ul>
        </li>
        <li>In summary, base-10 (decimal) notation consists of ten possible digits, and the number of possible combinations for an n-digit decimal number is $10^n$. This makes decimal notation essential for everyday arithmetic and provides a familiar framework for understanding numerical concepts.</li>
        <li>If you are working with 8 bits (each bit is a place that could be use as 0 or 1) then the number of possible combinations you could achieve is 256. The maximum number you could create with 8 bits is 255 (0-255 - 256 possible combinations- ). 11111111 is 255 in base-2 with 8 bits.</li>
        <li>A byte is 8 bits. This means that a megabyte is a million bytes, a gigabyte is a billion bytes.</li>
        <li>Most computers today have a 32-bits or 64-bits that means that the computer are operating in chunks of 32 or 64 bits.</li>
        <li>To represent the sign of the number, most computers use the first bit to represent the sign (0 negative and 1 positive) and the next 31 bits for the numbers. That would give you  +-2^31 combinations (-2147483648, 2147483647 )</li>
        <li></li>
        <li></li>
        <li><u><b>But what about numbers with commas?</b></u></li>
        <li>They are called floating numbers and are represented in memory like this.</li>
        <li>If you want to represent 625.9</li>
        <li></li>
        <li><u><b>What about letters?</b></u></li>
        <li>You represent it with numbers.</li>
        <li>ASCII and Unicode are character encoding standards used to represent text characters digitally.</li>
        <li>1. <b>ASCII</b>:
            <ul>
                <li>ASCII represents text characters using 7 bits, allowing for 128 (2^7) possible combinations.</li>
                <li>It assigns numerical values (0 to 127) to characters, primarily for English text.</li>
                <li>ASCII is limited in supporting only English characters and symbols.</li>
            </ul>
        </li>
        <li>2. <b>Unicode</b>:
            <ul>
                <li>Unicode is a character encoding standard supporting characters from all languages and writing systems.</li>
                <li>It assigns unique numerical values to each character, enabling multilingual text representation.</li>
                <li>It uses 16 bits.</li>
                <li></li>
            </ul>
        </li>
        <li><b>How computers calculate: ALU </b></li>
        <li>An Arithmetic Logic Unit (ALU) is a fundamental component of a computer&#39;s central processing unit (CPU). It is responsible for performing arithmetic and logical operations on data that is being processed by the CPU. These operations include addition, subtraction, multiplication, division, AND, OR, and NOT operations. The ALU takes input from the CPU&#39;s registers, performs the requested operation, and then outputs the result back to the CPU. ALUs are crucial for executing computational tasks and manipulating data within a computer system.</li>
        <li></li>
        <li>The ALU has 2 units: arithmetic unit and a logic unit.</li>
        <li>Arithmentic unit  </li>
        <li>Is the responsible for handling all numerical operations in a computer.
Let&#39;s add two binary numbers together. In the binary system, there are only for possibilities: 0</li>
        <li></li>
        <li>1. 0 + 0 = 0</li>
        <li>2. 0 + 1 = 1</li>
        <li>3. 1 + 0 = 1</li>
        <li>4. 1 + 1 = 0 (you carry the 1 to the next sum)</li>
        <li></li>
        <li>The table needed for this sum is exactly like the xor gate, which means we can use it and modify it to suit our needs. This circuit is called a half-adder. It has two inputs (a, b) and two outputs (the sum and the carry value )</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FJvRJd59EtwAUMpy6uhL7FXDgwy0apF2piOBiUnNVf4Q_zcl8_anG8n7XY2l4URDhrLWMLx3n7fkbMHQkGdCUN05TPrJm7Y0D4by6jyW8dTEp5pyoLmXfWH_G0jNiuW1H.png" width="741" height="658"/></li>
        <li></li>
        <li>You will have a problem, the next time you have to add two numbers, and you have to carry one, you will have to add 3 numbers instead. You have to build a full-adder</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F-q6IvaJjH-xNZqcGKaCo5TwiuigQV0Kbs-yCvDnFgma41pUT1_28LDc2iQEQ-Hep2hlVgYC-AoDVPZDjxXMUrZ6mRhqPKuJFbBsCLGxMCNnbQRSGXM_p4XS0proV2bnP.png" width="346" height="301"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FsMeljOED6jyt2VMs8EdY_QO4SVdPawb71TNTBAssWqakloiYLRPzPqgj9Ul_f0xwVFaKp_18BIUhYTuT2VkGsg7Dke-WbesdnHo22y0nswMpVPnTXhmQY0TwNED9RnX-.png" width="790" height="236.01250000000002"/></li>
        <li>You have 3 inputs per addition and two results, the sum of the 3 numbers and if you have to carry 1.</li>
        <li></li>
        <li>And then to create an  8-bit sum.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FLBWQrr5-xjmXUyG227UHCTbEjNSIgQH7udApJFLAJej0m-5GtFYJI3fP8KtvtY5RDXyoBWrccniJQQalB1ghsMdVyp0kvhJMKBS__CwKZxChCmmIJy5Y3PvcnHVeJ_Q8.png" width="790" height="392.0375"/></li>
        <li>An overflow happens when the last carry value is 1, which means that 8 bits would not be enough to represent the result, and the sum will probably return an error.</li>
        <li></li>
        <li></li>
        <li>Logic unit  </li>
        <li>The logic unit in the ALU performs logical operations such as AND, OR, and NOT on binary inputs. It combines input bits according to specified logic operations and produces corresponding output bits. These logical operations are essential for decision-making and data manipulation within the CPU during arithmetic and logical computations.</li>
        <li></li>
        <li></li>
        <li>Finally, you will want to create a new level of abstraction that allows you to think in more high level terms. In this case, you will have the entire ALU.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FhTfeNDalLe7YzuSTMIt2LaSJfYCl8h5_elBz6yfSo71rIOiP4aUjgNeAo1F4VhhnIdRRDLXVk7iutYvc9W5OLNWasp0_IF3joQIf87kWLWwH6ODwwKqOXVjNqcsQMDoh.png" width="790" height="409.8125"/></li>
        <li></li>
        <li></li>
        <li><b>Registers and RAM</b></li>
        <li>How to use logic circuits to create memory?</li>
        <li>There are two logic circuits that are really useful to save data and create memory. They are called a and-or latch and a gated latch, the first one is to explain and the second one is used in RAMs.</li>
        <li>Basically the AND-OR latch circuit allows you to save a 0 or 1 into a circuit.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FEXBeZTIijglYtlbJUgrnkQImGOhF0okE-qXByhVZ3kQtJH4itAQOcM1MzsBfSzEW1RQbMJvPINJokim2QbtN25Cr5Q1RzXHJbLTWirV57Amv_phjLPYM1L2ubWZYXI6s.png" width="790" height="255.76250000000002"/></li>
        <li></li>
        <li></li>
        <li>The gated-latch is more complete and allows you to control if the change can be done or not with a write enable circuit attatched to a circuit that stores a bit.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F2VWSy6Jg4Qr7uSICq756akPKBQis22pu0YJz8ChedH1c0DM5qmoao6GGaleDd5O535bly15SWLysPziP9Uoduawb27ZTS9zt85gR0EP0_LTgDY8zUQyh9ttw0bIFUxCY.png" width="790" height="255.76250000000002"/></li>
        <li></li>
        <li>If you put 8 latches side by side you can store 8 bits of information or a byte, like an 8bit number. A group of latches operating like this is called a register, which holds a single number. Today you have registers of 32bits or 64bits</li>
        <li></li>
        <li></li>
        <li>Now let&#39;s build something that can store more data. To do this we can use a matrix.</li>
        <li>16x16 latch matrix</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FXgaPX4n2uYNGyPqBkjhYtm1HTa1ULoNuqqzkO8dDuF6aRxf6r8oS3azOi0kFdq64_jH5zfq_1FCdnreFcR_cMCyDTV7szx19oTVEJ_u6Cz6EXPsJUrJ2v5Kb82ghbZUq.png" width="790" height="426.6"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FmLAc3UVofpK9z52cxorm0M-Zl_uo2huKig1xhawGaZ1EESe8pxpVBkXECIxRm1ijCOFMSorv8q4zwr2W7uA4qkiLXhJLU2Ni2ZLmHHJFBA0uhCOYmvbjmx4OTR0bAjCV.png" width="790" height="490.7875"/></li>
        <li>This way you use the same wires you will use for every gated latch for data in/out and write enable and read enable, because the wires that select the latch will only cross one latch at a time (row - column).</li>
        <li>This way for 256 bits of memory you will only need 35 wires:</li>
        <li>1 data wire</li>
        <li>1 write enable wire</li>
        <li>1 read enable wire</li>
        <li>16 for rows</li>
        <li>16 for columns</li>
        <li></li>
        <li>Memory address  </li>
        <li>The data stored in each latch will have an address to access it later. This address will be saved with 8 bits, 4 bits for the row address (2^4 = 32 possibilities and we only have 16 rows) and 4 for the column. Let&#39;s say we want to read the data in the latch row 12 and column 8, that would be 11001000 (1100 = 12, 1000 = 0). The component that receives the address and selects the row and column is called multiplexer (you select the row and the column and then you perform the operation).</li>
        <li>If you add the matrix and the multiplexer with all of the other stuff we have talked about you have a 256 bit memory component. This component will need 8 wires to share the address, a write enable wire, a read enable wire and a data wire.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fdjjz0s7qHSM2RMvj8LvWL8fODYw-mFlmwsR6zjefU007uDN5ubArzQ6G2qbPK6VlNEJtSBoqwn9U7CTTP6L5pKbiO5IKfYRBaPPUznF7xp62fJ1kCQNoV7LaX1PzwLm7.png" width="675" height="410"/></li>
        <li></li>
        <li>To scale this up, we need to put them 8 of them in a row.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FqRqcyaJyfa_KrWaHsjgEdzwZeVYm4gL98WwZXKZT3iCZJyy_jzvOs-HFbrO0Yc2ASnRFzsRqAp_FQw5dzLJr1WXxHDVP1Ehf9RmV_kvVxa8ls371tfPFA1HyVYTL-z43.png" width="790" height="354.5125"/></li>
        <li>This way if you want to store an 8bit number you:</li>
        <li>Turn on the write enable wire</li>
        <li>Send the memory address of the number you want to store and the multiplexer will select the same latch in every 256-bit memory component.</li>
        <li>Give one bit of data wire to each of the 8 components of 256-bit memory.</li>
        <li>Store one bit of data in each component.</li>
        <li>Then if you want to retrieve the number send the memory address and the system will return bit by bit your number.</li>
        <li>Let&#39;s say that you want to store the number 11001110. This component will:</li>
        <li>Turn the write enable wire</li>
        <li>Save the first bit (1) in the first 256-bit memory component  in the address rc (row-column).</li>
        <li>Save the second bit (1) in the second 256-bit memory component  in the address rc (row-column).</li>
        <li>Save the third bit (0) in the third 256-bit memory component  in the address rc (row-column).</li>
        <li>...</li>
        <li>Save the eight bit (0) in the eight 256-bit memory component  in the address rc (row-column).</li>
        <li>turn off the write enable wire.</li>
        <li></li>
        <li>Let&#39;s say that you want to retrieve the number in the address 11001000. This component will:</li>
        <li>Specify the address (row-column) from which you want to retrieve the information.</li>
        <li>Turn on the read enable wire to allow reading from the memory components.</li>
        <li>Access the specified address in each of the 256-bit memory components.</li>
        <li>Retrieve the bit stored at each address in sequence, from the first to the eighth component.
            <ul>
                <li>Retrieve the bit stored in the first 256-bit memory component at the address rc (row-column).</li>
                <li>Retrieve the bit stored in the second 256-bit memory component at the address rc (row-column).</li>
                <li>Retrieve the bit stored in the third 256-bit memory component at the address rc (row-column).</li>
                <li>...</li>
                <li>Retrieve the bit stored in the eighth 256-bit memory component at the address rc (row-column).</li>
            </ul>
        </li>
        <li>Assemble the retrieved bits into the desired data format (e.g., binary, decimal, etc.).</li>
        <li>Turn off the read enable wire once retrieval is complete.</li>
        <li></li>
        <li>We will concieve it like this:</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fg0lTtJD6ZlCwfdm7_jWhQj6aaGobMVSXWzjYzuaWdhNnKrSBXaBaqpMS1E89bX1rG3573XASODbi_PQWducHa9Y3sZ9ZGtzdOrcjSSdMzOquhAh73jpUPCvGr4zIorok.png" width="673" height="638"/></li>
        <li>Basically if the cpu says &quot;bring the address 12&quot; it will execute everything above and bring the entire 8-bit number.</li>
        <li></li>
        <li>Let&#39;s see a real computer now.</li>
        <li>What is a RAM?   </li>
        <li>RAM (Random Access Memory) in a computer serves as temporary storage for data and program instructions that the CPU (Central Processing Unit) needs to access quickly. It allows the CPU to rapidly retrieve and store information for immediate use, facilitating smooth and efficient operation of programs and processes. RAM is volatile memory, meaning it loses its data when power is turned off, unlike storage devices such as hard drives or SSDs which retain data even when the power is off.</li>
        <li></li>
        <li>This a stick of RAM with 8 memory modules solded onto the board.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F2prZA-CerM0qMa6giANPPKMEneCK4WT9PoOQwlOe7W-ib0_LfUtHGKhL46mVjp2GAMzH6veiCvYcfKB_icT7mBbswrC6qtbiCY0_iH7n3YvBdJyOep_WGuJHpgymlYli.png" width="790" height="185.65"/></li>
        <li>If you zoom in, every memory module looks like this. This one has 32 squares of memory.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FnUPX5y_Er016J6df_gqg9AFJFTRLOoH0Kw4GCajHShNuegQzYIob3d39aFRGgFMI4PV4MzcAC_vnWcGTjTATDSSMTCrUVTkryaDhuL-WTVgWwBWkBnDVGKfKLm7YQrmf.png" width="790" height="432.52500000000003"/></li>
        <li></li>
        <li>If you zoom in each square of memory you will see that each one is composed of 4 blocks</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F9BxISSuQmMn6mZEzMPmJOXDY6dqQ0SBydMrRamgsrVIume1SCBJpJ7MjvO1jCGvatuM-y5125CBt_DTxfUYizfYKhM30esmHFkft359GjltKJ6m4jG-63S8s-4ssSQfi.png" width="790" height="432.52500000000003"/></li>
        <li>And if you zoom again, you get down into the matrix of individual bits. This is a matrix of 128x64 bits. That&#39;s 8192 bits in total. If you do the math you will see:</li>
        <li>8192 * 4 blocks = 32768.</li>
        <li>Each chip has 32 squares which means 32 * 32768 = 1048576</li>
        <li>Each stick (ram module) of memory has 8  chips which means 8 * 1048576 = 8388608 bits = 1 megabyte</li>
        <li></li>
        <li></li>
        <li></li>
        <li><b>The central processing unit (CPU)</b></li>
        <li>What is the CPU and what does it do?</li>
        <li>A CPU&#39;s job is to execute programs.</li>
        <li>Programs are made up of a series of individual operations called instructions (because they instruct the computer what to do)</li>
        <li></li>
        <li>Let&#39;s give the processor 4 8-bit memory registers which will be used to temporarily store and manipulate values.</li>
        <li>Programs can be stored in memory too.</li>
        <li>We assign an ID to each instruction supported by our cpu</li>
        <li>The first column is the ID of the instruction</li>
        <li>The third column is the 4-bit operation code</li>
        <li>The fourth column is the Address or Register specifies where the DATA for that operation should come from. So you have an operation to do with x and y data</li>
        <li>The first column tells you which operation you want to do</li>
        <li>The third one tells you how to tell the machine which operation to do</li>
        <li>The fourth column tells the pc where to get the data for that operation.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F-DTrpEGonS67ZKWMSXZ0DXv164AaP6Gfsbkxc3KfMr8qwYutCAthC8OoIlKRLQfR-w0MlWVvza5f2LuAAzLVXlAyDbjTQ74_xlQOkC0SkK_eD4xSHVw7R4onDcgFyOWp.png" width="790" height="346.6125"/></li>
        <li></li>
        <li></li>
        <li><u><b>To create a CPU we need:</b></u> </li>
        <li>A stick of ram</li>
        <li>4 memory registers to store and manipulate data temporarily</li>
        <li>1 register to keep track where we are in a program, called an &quot;instruction address register&quot;. Basically stores the memory address of the current instruction.</li>
        <li>1 register to store the current instruction called a &quot;instruction register&quot; (NOT THE MEMORY  ADDRESS OF THE CURRENT INSTRUCTION)</li>
        <li></li>
        <li></li>
        <li>Computer stage/phase </li>
        <li>In the first phase of the cpu&#39;s operations is called the &quot;fetch phase&quot;</li>
        <li><u><b>Fetch:</b></u></li>
        <li>CPU retrieves instructions from computer memory (RAM).</li>
        <li>Instructions are stored sequentially in memory.</li>
        <li>CPU fetches instructions based on the program counter (instruction address register IAR) .</li>
        <li>Example:</li>
        <li>Let&#39;s say that the IAR says &quot;00001000&quot;. The cpu retrieves the data from the RAM in that address and places it in the IR (instruction register).</li>
        <li><u><b>Decode:</b></u></li>
        <li>CPU interprets the binary instruction code.</li>
        <li>CPU divides the number in two: the first 4 bits are the OPCODE (operation code) and the next 4-bits are the RAM memory address of the data the operation requires.</li>
        <li>The Control unit decodes and interprets the instructions. It does not have a logic gate to check each operation code, it&#39;s more complex than that, but in the image we will exemplify with an individual logic gate to simplify. In real case scenarios it does not make sense to have 300 individual logic gates (circuits) and make each operations code to run through all of them to check which one is equal, instead, they have complex circuits which output corresponds with the wire that will execute the operation code (or something like that, technically it sends a signal that makes the execute phase know which actions has to take or something like that).</li>
        <li><u><b>Execute:</b></u></li>
        <li>CPU carries out the operation specified by the decoded instruction.</li>
        <li>Can involve arithmetic or logical calculations, data movement, or control transfer.</li>
        <li>May access data from memory or perform other operations required by the instruction.</li>
        <li>After execution, the cycle repeats with the CPU fetching the next instruction from memory. The Instruction adress Register acts like an accumulator and adds one to the number it has. This continuous cycle enables the CPU to execute a series of instructions, performing complex computations and tasks required by the program.</li>
        <li></li>
        <li><u><b>Example step by step:</b></u></li>
        <li>Assumptions:</li>
        <li>The CPU has separate registers for A, B, and an Instruction Register (IR).</li>
        <li>The RAM is used to store both data and instructions.</li>
        <li>The ALU (Arithmetic Logic Unit) performs arithmetic operations.</li>
        <li></li>
        <li>1. <b>LOAD_A:</b></li>
        <li><b>Clock cycle 1-3:</b>
            <ul>
                <li><b>Fetch:</b>
                    <ul>
                        <li>The Instruction Address Register (IAR) contains the address of the next instruction.</li>
                        <li>The Control Unit fetches the instruction from the RAM at the address specified by the IAR.</li>
                        <li>The fetched instruction is stored in the Instruction Register (IR).</li>
                    </ul>
                </li>
                <li><b>Decode:</b>
                    <ul>
                        <li>The Control Unit interprets the instruction in the IR as LOAD_A.</li>
                        <li>It sets the necessary control signals to prepare for executing this instruction.</li>
                    </ul>
                </li>
                <li><b>Execute:</b>
                    <ul>
                        <li>The Control Unit signals the RAM to fetch the data from the memory address specified in the instruction.</li>
                        <li>The data is loaded into the A register.</li>
                    </ul>
                </li>
            </ul>
        </li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F2nOjcZwb5Ao6nLQwzsfJT7y_CoP8JJbV1oY_8u8V1Yzku-fi68Q0t-YQLkMP9jcyPF3DdccZPOq0QNL9jObm9sqcSHVNLCvFijmUGyVYvWIoRdkVsTPU0pvOJt6cQBQ9.png" width="790" height="467.08750000000003"/></li>
        <li></li>
        <li>2. <b>LOAD_B:</b></li>
        <li><b>Clock cycle 4-6:</b>
            <ul>
                <li><b>Fetch:</b>
                    <ul>
                        <li>The Control Unit increments the IAR to point to the next instruction.</li>
                        <li>It fetches the next instruction from RAM into the IR.</li>
                    </ul>
                </li>
                <li><b>Decode:</b>
                    <ul>
                        <li>The Control Unit identifies the instruction as LOAD_B.</li>
                        <li>Control signals are set accordingly.</li>
                    </ul>
                </li>
                <li><b>Execute:</b>
                    <ul>
                        <li>The Control Unit instructs the RAM to retrieve the data from the specified memory address.</li>
                        <li>The retrieved data is loaded into the B register</li>
                    </ul>
                </li>
            </ul>
        </li>
        <li>The same as the image before but with register B</li>
        <li>3. <b>ADD:</b></li>
        <li><b>Clock cycle 7-9:</b>
            <ul>
                <li><b>Fetch:</b>
                    <ul>
                        <li>The Control Unit increments the IAR to get the next instruction.</li>
                        <li>It fetches the instruction from RAM into the IR.</li>
                    </ul>
                </li>
                <li><b>Decode:</b>
                    <ul>
                        <li>The Control Unit recognizes the instruction as ADD.</li>
                        <li>In this case we have a 2 2-bit RAM ADDRESS (look up in the operations code list), which means that we can select 2 of the 4 registers we have. The first 2-bits for the register B and the next for the A.</li>
                        <li>Necessary control signals are set.</li>
                    </ul>
                </li>
                <li><b>Execute:</b>
                    <ul>
                        <li>The Control unit enables register b and feeds its value to input 1</li>
                        <li>The Control unit enables register a and feeds its value to input 2</li>
                        <li>The control unit configures the ALU passing the operation code</li>
                        <li>The output goes to a temporary memory register inside the Control unit</li>
                        <li>The control unit stores the register A value</li>
                    </ul>
                </li>
            </ul>
        </li>
        <li></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FOyfIXn-nMOmM5LF820PSZ5w2pGab2wWphXF9GVHj7ytMpMWZWeRRGPTZIfvcOr61vCFFoIHqY1LWCWfCfQpKXuiWb9VEjT56zJBlcufSkaZmsG5OW2INclsy2XI6sHHO.png" width="790" height="402.90000000000003"/></li>
        <li></li>
        <li>4. <b>STORE_A:</b></li>
        <li><b>Clock cycle 10-12:</b>
            <ul>
                <li><b>Fetch:</b>
                    <ul>
                        <li>The Control Unit increments the IAR.</li>
                        <li>It fetches the next instruction from RAM into the IR.</li>
                    </ul>
                </li>
                <li><b>Decode:</b>
                    <ul>
                        <li>The Control Unit identifies the instruction as STORE_A.</li>
                        <li>Control signals are set accordingly.</li>
                    </ul>
                </li>
                <li><b>Execute:</b>
                    <ul>
                        <li>The Control Unit instructs the RAM to store the content of register A into the specified memory address.</li>
                    </ul>
                </li>
            </ul>
        </li>
        <li>At the end of the execution, the process is complete, and the result of the addition is stored in RAM or any other specified location. This sequence demonstrates the fundamental steps involved in executing instructions on a simple 8-bit CPU with RAM. Each instruction goes through fetch, decode, and execute phases, with one action per stage.</li>
        <li></li>
        <li>What is the control unit of a cpu?  </li>
        <li>The control unit is a crucial component of a CPU (Central Processing Unit). It&#39;s responsible for coordinating the activities of the other hardware components within the CPU and ensuring that instructions from computer programs are executed in the correct sequence.</li>
        <li>Here are some key points about the control unit:</li>
        <li>1. <b>Instruction Interpretation</b>: The control unit interprets the instructions fetched from memory during the fetch phase of the CPU cycle. It decodes these instructions to determine the specific operation that needs to be performed.</li>
        <li>2. <b>Instruction Execution</b>: Once instructions are decoded, the control unit coordinates the execution of these instructions. It directs the necessary arithmetic, logical, or data transfer operations within the CPU to carry out the instruction&#39;s specified task.</li>
        <li>3. <b>Sequencing and Timing</b>: The control unit manages the sequencing and timing of operations within the CPU. It ensures that instructions are executed in the correct order and that each operation occurs at the appropriate time.</li>
        <li>4. <b>Control Signals</b>: The control unit generates control signals that regulate the flow of data between different CPU components, such as registers, ALU (Arithmetic Logic Unit), and memory. These control signals facilitate the movement of data and the execution of instructions.</li>
        <li>5. <b>Synchronization</b>: In multi-core CPUs, where multiple processing cores are present, the control unit helps synchronize the activities of these cores to ensure efficient processing and avoid conflicts between tasks.</li>
        <li>Overall, the control unit acts as the &quot;brain&quot; of the CPU, orchestrating its various components to execute instructions and perform computations according to the program&#39;s requirements. It plays a crucial role in the overall functioning and performance of the CPU.</li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li>CPU&#39;s clock  </li>
        <li>The &quot;clock&quot; of a CPU refers to its internal timing mechanism, which regulates the rate at which the CPU executes instructions. This clock signal sets the pace for the CPU&#39;s operation, defining the intervals at which it processes data and executes instructions. The clock speed, usually measured in hertz (Hz), represents the frequency at which this internal clock oscillates.</li>
        <li>For example, if a CPU has a clock speed of 3.0 gigahertz (GHz), it means that the internal clock of the CPU cycles at a rate of 3.0 billion times per second. Each cycle of the clock typically corresponds to a basic unit of work that the CPU can perform, such as fetching an instruction, decoding it, executing it, and storing the result.</li>
        <li></li>
        <li>Other definitions</li>
        <li>1. <b>Clock Signal</b>: The CPU&#39;s clock signal is a regular, periodic waveform that oscillates between high and low voltage states at a constant frequency. This frequency, measured in Hertz (Hz), determines the rate at which operations are synchronized and controlled within the CPU.</li>
        <li>The clock signal sets the rhythm or pace at which the CPU operates. It determines the timing and frequency of execution, effectively dividing time into discrete intervals or cycles. Each cycle corresponds to a specific amount of time during which a set of operations can occur.</li>
        <li>2. <b>Clock Cycle</b>: The clock cycle represents one complete pulse of the CPU&#39;s clock signal. It defines the basic unit of time for the CPU&#39;s operations and sets the pace at which instructions are processed.</li>
        <li>3. <b>Pipeline</b>: The CPU&#39;s pipeline breaks down the execution of instructions into multiple stages, such as fetch, decode, execute, and write back. Each stage of the pipeline represents a distinct operation or task within the instruction processing cycle. This allows to execute more than one action at a time. Instructions  that would usually take 3 (or more, depending on the cpu) stages, don&#39;t finish before the next instruction is fetched, rather the cpu moves the fetched instruction to the decode phase, and fetches a new instruction, creating a flow in the pipeline.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FFS1rkk4Yd55IuP80FME2qdwrO-Qq-l_pD4oFWwNoKrleCYmFttZBPrYqKJKFWUy39sk2rXzu7clUn4Sgy1eiZzvst35EAspsZtm23-X6iu98wApejh7gTHY8mCuDDigT.png" width="790" height="328.83750000000003"/></li>
        <li>4. <b>Concurrency</b>: Within the pipeline, multiple instructions can be in different stages of execution simultaneously, allowing for overlap and parallelism of operations. This concurrency helps improve CPU efficiency and throughput.</li>
        <li>5. <b>Pipeline Stalls</b>: When an operation within the pipeline takes longer than a single clock cycle to complete, the pipeline may stall or pause temporarily. During a stall, the pipeline remains idle until the lengthy operation finishes, maintaining synchronization with the CPU&#39;s clock signal.</li>
        <li>6. <b>Clock Frequency and Performance</b>: The CPU&#39;s clock frequency, combined with the efficiency of its architecture and pipeline design, determines its overall performance. Higher clock frequencies generally allow for faster instruction processing, while efficient pipelining and optimization techniques help maximize CPU throughput and efficiency.</li>
        <li></li>
        <li></li>
        <li>La Computadora, Arquitectura de Von Neumann</li>
        <li>Summary  </li>
        <li>The Von Neumann architecture, named after Hungarian-American mathematician and physicist John von Neumann, is a theoretical framework for a computer&#39;s design that is still widely used today. It&#39;s the basis for almost all modern computers, including desktops, laptops, smartphones, and servers.</li>
        <li>The key components of the Von Neumann architecture are:</li>
        <li>1. <b>Central Processing Unit (CPU):</b> This is the brain of the computer. It executes instructions fetched from memory, performs arithmetic and logic operations, and controls the flow of data within the system.</li>
        <li>2. <b>Memory:</b> In the Von Neumann architecture, both instructions and data are stored in the same memory unit. This memory is typically divided into two types: RAM (Random Access Memory) for temporary storage of data and instructions currently being processed by the CPU, and storage (such as a hard drive or solid-state drive) for long-term storage of data and programs.</li>
        <li>3. <b>Control Unit (CU):</b> The control unit manages the flow of instructions within the CPU. It fetches instructions from memory, decodes them, and executes them in sequence.</li>
        <li>4. <b>Arithmetic Logic Unit (ALU):</b> This component performs arithmetic and logic operations on data. It&#39;s responsible for tasks like addition, subtraction, multiplication, division, and comparisons.</li>
        <li>5. <b>Input/Output (I/O) System:</b> This system handles communication between the computer and external devices, such as keyboards, mice, monitors, and printers. It allows the computer to send and receive data to and from these devices.</li>
        <li>The Von Neumann architecture is characterized by its <b>&quot;stored-program concept,&quot;</b> which means that both program instructions and data are stored in memory, and the CPU fetches instructions from memory sequentially to execute them. This is in contrast to earlier computing models where programs were hard-wired into the machine and couldn&#39;t be easily changed.</li>
        <li>One of the main advantages of the Von Neumann architecture is its flexibility. Since programs and data are stored in the same memory, it&#39;s relatively easy to write new programs and modify existing ones. This makes it well-suited for general-purpose computing tasks.</li>
        <li>However, this architecture also has limitations. For example, the Von Neumann bottleneck refers to the fact that the CPU can only fetch and execute one instruction at a time, which can limit performance in some scenarios. Additionally, the shared memory design can lead to security vulnerabilities, as it&#39;s possible for malicious programs to alter the instructions being executed or access sensitive data in memory.</li>
        <li>Overall, the Von Neumann architecture is a fundamental concept in computer science and serves as the basis for understanding how modern computers are designed and operate.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fcn0A6m7ARvY-SyQyzHlGtSh4gJmsnJFL2pfM5D26_0VT3J5enHiXe2XBujEesR3UyFjVHF6AZ58cVihnoXimFAkEtvzciSH83d9n6i6FmPJHedSthOkcfP5HxelNkDx9.svg" width="510" height="295"/></li>
        <li></li>
        <li>Development  </li>
        <li>The first generation of computers utilized vacuum tubes for digital logic elements and memory. The IAS computer, a prominent first-generation computer, introduced the stored-program concept, attributed to mathematician John von Neumann and concurrently developed by Alan Turing. This concept was first proposed in von Neumann&#39;s 1945 EDVAC proposal. The IAS computer was designed by von Neumann and his colleagues at the Princeton Institute for Advanced Studies, completed in 1952, and served as the blueprint for subsequent general-purpose computers.</li>
        <li><b>The structure of the IAS computer includes:</b> </li>
        <li>Main memory storing both data and instructions.</li>
        <li>An arithmetic and logic unit (ALU) capable of binary data operations.</li>
        <li>A control unit interpreting and executing instructions stored in memory.</li>
        <li>Input-output (I/O) equipment operated by the control unit.</li>
        <li></li>
        <li></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FITRrv7EjO2WjKQvxDALnOcUtF_nunZPWBEBGfT1ukQO3kgCjIhG8DGZYXFqr0vzMOZVF6Zo2LBSt1vbZ_jl3MRgyWCSBCGvb7JcuvfEPBpyUkGjK_S5rUKUHZBRevtaV.png" width="790" height="791.975"/></li>
        <li><b>Memory Buffer Register (MBR):</b>
            <ul>
                <li>Contains a word to be stored in memory or sent to the I/O unit.</li>
                <li>Used to receive a word from memory or from the I/O unit.</li>
            </ul>
        </li>
        <li><b>Memory Address Register (MAR):</b>
            <ul>
                <li>Specifies the address in memory of the word to be written from or read into the MBR.</li>
            </ul>
        </li>
        <li><b>Instruction Register (IR):</b>
            <ul>
                <li>Contains the 8-bit opcode instruction being executed.</li>
            </ul>
        </li>
        <li><b>Instruction Buffer Register (IBR):</b>
            <ul>
                <li>Employed to temporarily hold the right-hand instruction from a word in memory. The difference between the IBR and the IR is that the IBR fetches the instruction from memory and stores it, that instruction is not being decoded and nothing is being done with it. When the IR is ready to get another instruction, the IBR sends the stored instruction to the IR, where it is decoded, etc.</li>
            </ul>
        </li>
        <li><b>Program Counter (PC):</b>
            <ul>
                <li>Contains the address of the next instruction pair to be fetched from memory.</li>
            </ul>
        </li>
        <li><b>Accumulator (AC) and Multiplier Quotient (MQ):</b>
            <ul>
                <li>Employed to temporarily hold operands and results of ALU operations.</li>
                <li>For example, when multiplying two 40-bit numbers, the result is an 80-bit number. The most significant 40 bits are stored in the AC, and the least significant bits are stored in the MQ.</li>
            </ul>
        </li>
        <li></li>
        <li></li>
        <li></li>
        <li>Why does the MBR connect with the I/O processes?  </li>
        <li>The I/O (Input/Output) operations often involve transferring data between the CPU and external devices, such as storage units, network interfaces, or peripherals like printers and keyboards. The Memory Buffer Register (MBR) is involved in these operations because it serves as a temporary storage location for data during data transfers between the CPU and memory, or between the CPU and I/O devices.</li>
        <li>Here&#39;s why the I/O operations work with the MBR:</li>
        <li>1. <b>Data Transfer:</b> When data needs to be moved between the CPU and memory or between the CPU and an I/O device, it passes through the MBR. The MBR acts as a buffer, temporarily holding the data during the transfer process.</li>
        <li>2. <b>Versatility:</b> The MBR is designed to handle various types of data transfers. It can store data that is being read from memory or an I/O device before it&#39;s processed by the CPU. Similarly, it can hold data that the CPU wants to write into memory or send to an I/O device.</li>
        <li>3. <b>Interface:</b> The MBR serves as an interface between different components of the computer system. It allows the CPU to communicate with memory and I/O devices efficiently by providing a standardized location for data to be temporarily stored during transfer operations.</li>
        <li>4. <b>Efficiency:</b> By using the MBR as an intermediate storage location, the CPU can continue executing instructions while data transfers are in progress. This improves overall system efficiency by minimizing the idle time of the CPU.</li>
        <li>In summary, the MBR is an integral part of the data transfer process in a computer system, serving as a temporary storage location for data during I/O operations between the CPU, memory, and external devices.</li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li>How do the MBR and MAR work together?  </li>
        <li>The Memory Buffer Register (MBR) and Memory Address Register (MAR) work together in the process of transferring data between the CPU and memory in a computer system.</li>
        <li>Here&#39;s how they collaborate:</li>
        <li>1. <b>Data Transfer Initialization:</b>
            <ul>
                <li>When the CPU needs to read data from or write data to a specific memory location, it first loads the memory address into the MAR. The MAR holds the address of the memory location where the data transfer will occur.</li>
            </ul>
        </li>
        <li>2. <b>Data Transfer Execution:</b>
            <ul>
                <li>Once the memory address is loaded into the MAR, the CPU initiates the data transfer process. The data to be transferred is either fetched from memory or sent to memory, depending on the operation being performed.</li>
                <li>During this process, the MBR serves as a temporary storage location for the data being transferred. If data is being read from memory, it is temporarily stored in the MBR before being processed by the CPU. Similarly, if data is being written to memory, it is first loaded into the MBR before being written to the specified memory location.</li>
            </ul>
        </li>
        <li>3. <b>Completion and Result:</b>
            <ul>
                <li>After the data transfer is completed, the CPU can access the data in the MBR for further processing, such as arithmetic or logic operations.</li>
                <li>Once the operation is complete, the CPU may update the contents of the MBR or MAR as necessary for subsequent operations.</li>
            </ul>
        </li>
        <li>In summary, the MAR is responsible for holding the memory address where data is to be read from or written to, while the MBR acts as a temporary storage location for the data during the transfer process. Together, they facilitate efficient data transfer between the CPU and memory in a computer system.</li>
        <li></li>
        <li>Microprocesadores, subrutinas y lenguajes de bajo nivel </li>
        <li>Microprocessors</li>
        <li>Fundamental Components of a Digital Computer:  </li>
        <li>The basic elements of a digital computer, as we know, must perform data storage, movement, processing, and control functions. Only two fundamental types of components are required: gates and memory cells.</li>
        <li><b>Gates</b>: These devices execute Boolean or logical functions, controlling the flow of data similar to canal gates. Example: An <b>AND gate</b> produces output based on the truth values of its inputs (A and B).</li>
        <li><b>Memory Cells</b>: Responsible for storing binary data, each capable of holding a single bit in two stable states. There are many types, the function is just to store data.</li>
        <li></li>
        <li><u><b>Functions</b></u><u>:</u></li>
        <li><b>Data Storage</b>: Handled by memory cells.</li>
        <li><b>Data Processing</b>: Executed by gates, manipulating data based on input signals.</li>
        <li><b>Data Movement</b>: Enabled through pathways connecting memory cells and gates, facilitating information transfer.</li>
        <li><b>Control</b>: The paths among components can carry control signals. For example, a gate will have one or two data inputs plus a control signal input that activatesthe gate. When the control signal is ON, the gate performs its function on thedata inputs and produces a data output. Conversely, when the control signalis OFF, the output line is null, such as the one produced by a high impedance state. Similarly, the memory cell will store the bit that is on its input lead when the WRITE control signal is ON and will place the bit that is in the cell on its  output lead when the READ control signal is ON.  <u><b>PEDIRLE EXPLICACIÓN AL PROFESOR</b></u></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FmNmzUwKODjSzRnHtD-LJqnsCwrjFfwlNQivsNd8a5k-oR8x9tr7JyAL9rZIubCeKzvYp6LBtj-6YObmg6O6YzwoRyNrV3OSiucLo2qZodf1EC_g9rB5BbByFJciFJ1n8.png" width="790" height="290.325"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FSkaJWDwysqHQOMrZV0tWoBk0plSkup7FNDZjDs5JFLiKdlB4zcOYnpdFGVx47Nw6ZQYSgRDcagWk5DK0C-PcSekSNe00Oh4F4vf8OWnBrcQf7-oQYy0wRwPGt7-Ad-MI.png" width="610" height="619"/></li>
        <li></li>
        <li>What is a microprocessor? </li>
        <li>A microprocessor is a type of processor that contains all the components of a central processing unit (CPU) on a single chip. It is capable of executing general-purpose computing tasks and has evolved over time to become increasingly powerful and versatile.</li>
        <li>Before the advent of microprocessors, CPUs (Central Processing Units) were typically constructed using discrete components, meaning individual transistors, diodes, resistors, and other electronic components were assembled together on a circuit board to create the CPU&#39;s logic and processing functions. These CPUs were often large, power-hungry, and relatively slow compared to modern microprocessors.</li>
        <li>The Intel 8080 was the first general-purpose microprocessor. Introduced in 1974, it was designed to serve as the CPU for a wide range of computing applications, rather than being tailored to a specific use case like its predecessors. The 8080 offered improved performance, a larger instruction set, and greater versatility compared to earlier microprocessors such as the Intel 4004 and 8008, which were designed for specific applications like calculators and embedded systems. The Intel 8080 played a crucial role in the development of early personal computers and is considered a landmark in the history of microprocessor technology.</li>
        <li></li>
        <li>Microcontroller vs microprocessor  </li>
        <li>1. <b>Microcontroller</b>:
            <ul>
                <li>A microcontroller is a compact integrated circuit designed to perform specific tasks within a larger system.</li>
                <li>Microcontrollers are often used in embedded systems where the application requires a dedicated and optimized control mechanism.</li>
                <li>They are commonly found in devices such as washing machines, microwave ovens, remote controls, automotive systems, and various IoT devices.</li>
                <li>Microcontrollers are designed to execute specific tasks efficiently with minimal power consumption and cost.</li>
            </ul>
        </li>
        <li>2. <b>Microprocessor</b>:
            <ul>
                <li>It primarily focuses on executing instructions and performing arithmetic and logical operations.</li>
                <li>Microprocessors are commonly found in general-purpose computing devices such as personal computers, servers, laptops, tablets, and smartphones.</li>
                <li>They are designed to provide high performance and versatility, suitable for a wide range of applications.</li>
            </ul>
        </li>
        <li></li>
        <li>Things to know: microprocessors (maybe?)</li>
        <li>1. <b>Architecture</b>: Understand the basic architecture of a microprocessor, including components such as the arithmetic logic unit (ALU), control unit, registers, and data bus. Familiarize yourself with concepts like instruction fetching, decoding, and execution.</li>
        <li>2. <b>Instruction Set Architecture (ISA)</b>: Learn about different instruction sets such as Reduced Instruction Set Computing (RISC) and Complex Instruction Set Computing (CISC). Understand the types of instructions, addressing modes, and how instructions are encoded.</li>
        <li>3. <b>Registers</b>: Know the purpose and types of registers in a microprocessor, including general-purpose registers, special-purpose registers (like program counter, instruction register, stack pointer), and status flags.</li>
        <li>4. <b>Memory</b>: Understand how microprocessors access memory, including concepts like memory addressing, memory hierarchy (cache, RAM, ROM), and memory management techniques (virtual memory, paging).</li>
        <li>5. <b>Pipeline</b>: Learn about instruction pipelining and how it enhances processor performance by overlapping instruction execution stages. Understand pipeline hazards and techniques to mitigate them (such as forwarding and stalling).</li>
        <li>6. <b>Interrupts and Exceptions</b>: Understand how interrupts and exceptions are handled by the microprocessor. Learn about interrupt vectors, interrupt prioritization, and exception handling mechanisms.</li>
        <li>7. <b>Clock and Timing</b>: Understand the role of the system clock in synchronizing operations within the microprocessor. Learn about clock frequency, clock cycles, and how they impact the performance of the processor.</li>
        <li>8. <b>Parallelism</b>: Familiarize yourself with concepts of parallel processing, including instruction-level parallelism (ILP), thread-level parallelism (TLP), and multi-core architectures. Understand techniques such as pipelining, superscalar execution, and SIMD (Single Instruction, Multiple Data) processing.</li>
        <li>9. <b>Peripheral Interfaces</b>: Know about various peripheral interfaces commonly used with microprocessors, such as UART, SPI, I2C, USB, and Ethernet. Understand how these interfaces facilitate communication with external devices.</li>
        <li>10. <b>Application Areas</b>: Explore the diverse application areas of microprocessors, including personal computing, embedded systems, networking equipment, industrial automation, automotive electronics, and IoT devices.</li>
        <li>11. <b>Development Tools</b>: Familiarize yourself with development tools and environments used for microprocessor programming and debugging, such as assemblers, compilers, simulators, and debuggers.</li>
        <li>12. <b>Recent Trends</b>: Stay updated on recent advancements and trends in microprocessor design, including topics like power efficiency, security features, heterogeneous computing, and emerging architectures (such as neuromorphic and quantum computing).</li>
        <li></li>
        <li></li>
        <li>Subrutinas</li>
        <li>Subroutines on a CPU architecture work by allowing the execution of a block of code separate from the main program flow. Here&#39;s a summary of how subroutines function on a CPU:</li>
        <li>1. <b>Call</b>:
            <ul>
                <li>When a subroutine is called, the CPU transfers control to the starting address of the subroutine.</li>
                <li>This is typically done using a &quot;call&quot; instruction, which saves the address of the next instruction (the return address) onto the stack before transferring control.</li>
            </ul>
        </li>
        <li>2. <b>Execution</b>:
            <ul>
                <li>The CPU executes the instructions within the subroutine as specified by the program.</li>
                <li>The subroutine may perform various tasks, manipulate data, and execute logic based on its purpose.</li>
            </ul>
        </li>
        <li>3. <b>Return</b>:
            <ul>
                <li>Once the subroutine execution is complete, control is transferred back to the main program.</li>
                <li>This is typically done using a &quot;return&quot; instruction, which retrieves the return address from the stack and resumes execution from that point.</li>
            </ul>
        </li>
        <li>4. <b>Stack Manipulation</b>:
            <ul>
                <li>The CPU often uses a stack to manage subroutine calls and returns.</li>
                <li>The stack is used to store return addresses, parameters, and local variables.</li>
                <li>When a subroutine is called, the return address is pushed onto the stack. When the subroutine returns, the return address is popped from the stack to resume execution.</li>
            </ul>
        </li>
        <li>5. <b>Parameter Passing</b>:
            <ul>
                <li>Subroutines can accept parameters to customize their behavior.</li>
                <li>Parameters may be passed via CPU registers, stack parameters, or a combination of both.</li>
                <li>Parameters are typically passed before calling the subroutine and accessed within the subroutine using specific addressing modes.</li>
            </ul>
        </li>
        <li>6. <b>Local Variables</b>:
            <ul>
                <li>Subroutines may have local variables stored in CPU registers or memory locations.</li>
                <li>Local variables are used to store temporary data needed for the subroutine&#39;s execution.</li>
                <li>These variables are often allocated and deallocated within the subroutine&#39;s code.</li>
            </ul>
        </li>
        <li>7. <b>Interrupts and Exceptions</b>:
            <ul>
                <li>Subroutines are also used to handle interrupts and exceptions in CPU architectures.</li>
                <li>When an interrupt occurs, control is transferred to a specific interrupt service routine (ISR) subroutine.</li>
                <li>Similarly, exceptions trigger exception handling routines to handle errors or exceptional conditions.</li>
            </ul>
        </li>
        <li>Overall, subroutines allow for modular and structured programming by enabling code reuse, abstraction, and encapsulation of functionality within a CPU architecture. They play a crucial role in organizing and managing program logic at the low-level CPU level.</li>
        <li></li>
        <li>In low-level CPU architecture, such as assembly language programming, subroutines are still fundamental constructs, although they might be implemented differently compared to higher-level programming languages. At the CPU level, subroutines are typically implemented using concepts like branching, stack manipulation, and the instruction pointer.</li>
        <li></li>
        <li>how are subroutines  typically implemented at the CPU level?</li>
        <li>1. <b>Jump Instructions</b>: CPUs have instructions that allow them to jump to a specific memory address to execute instructions. This is often used to transfer control to the beginning of a subroutine.</li>
        <li>2. <b>Call and Return Instructions</b>: CPUs typically have instructions specifically designed for calling and returning from subroutines. The &quot;call&quot; instruction transfers control to a specified memory address, which typically contains the start of the subroutine. The &quot;return&quot; instruction transfers control back to the instruction immediately after the call instruction, effectively returning from the subroutine.</li>
        <li>3. <b>Stack Manipulation</b>: CPUs commonly use a stack to manage subroutine calls and returns. When a subroutine is called, the CPU typically pushes the current instruction pointer (the address of the next instruction to be executed) onto the stack. This allows the CPU to return to the correct location after the subroutine finishes executing.</li>
        <li>4. <b>Parameter Passing</b>: Parameters can be passed to subroutines in various ways, such as through CPU registers or the stack. For example, in x86 assembly language, parameters are often passed via registers like <q>eax</q>, <q>ebx</q>, etc., or pushed onto the stack before calling the subroutine.</li>
        <li>5. <b>Local Variables and Registers</b>: Subroutines may use local variables stored in registers or memory locations reserved for the subroutine&#39;s use. Some registers may be designated for specific purposes within subroutines, such as storing return values or other temporary data.</li>
        <li>6. <b>Interrupts and Exceptions</b>: Subroutines are also used to handle interrupts and exceptions in CPU architectures. When an interrupt occurs, the CPU typically transfers control to an interrupt service routine (ISR), which is essentially a special type of subroutine designed to handle the interrupt. Similarly, exceptions (such as division by zero or invalid memory access) can trigger exception handling routines.</li>
        <li>In assembly language programming, subroutines are often defined using labels to mark the entry and exit points of the subroutine. Jump and call instructions are then used to transfer control between different parts of the program.</li>
        <li>Overall, while the implementation details may vary depending on the specific CPU architecture and assembly language, the concept of subroutines remains essential for organizing and managing code at the low-level CPU level.</li>
        <li></li>
        <li>Lenguajes de bajo nivel</li>
        <li>What are Low Level Languages?  </li>
        <li>We call those languages as low level languages which are closer to hardware as compared to high-level languages instead of software. They provide little or no abstraction from the <a isInlineLink="true" href="https://www.geeksforgeeks.org/machine-instructions/">machine instructions</a> and that’s why they allow programmers to manipulate hardware elements like register, <a isInlineLink="true" href="https://www.geeksforgeeks.org/memory-management-in-operating-system/">memory</a> etc. Low-level languages are often used for designing systems, such as developing <a isInlineLink="true" href="https://www.geeksforgeeks.org/what-is-an-operating-system/">operating systems</a>, <a isInlineLink="true" href="https://www.geeksforgeeks.org/device-driver-and-its-purpose/">device drivers</a>, and <a isInlineLink="true" href="https://www.geeksforgeeks.org/introduction-of-embedded-systems-set-1/">embedded systems</a>.</li>
        <li></li>
        <li>Types of Low-Level Languages   </li>
        <li>Low level language are divided into two types.</li>
        <li><b>Machine Language</b>
            <ul>
                <li>We know that machines follow the language of binary system, means 0 and 1. Machine language is low level language which consists of binary codes which are directly operated by <a isInlineLink="true" href="https://www.geeksforgeeks.org/central-processing-unit-cpu/">CPU Central Processing Unit</a>. There every instruction are written in form of 0 and 1, so its very challenging for humans to understand and use as primary language.</li>
            </ul>
        </li>
        <li><b>Assembly Language</b></li>
        <li><a isInlineLink="true" href="https://www.geeksforgeeks.org/what-is-assembly-language/">Assembly language</a> is a way of writing computer programs that are very close to how the computer works. It have some symbols and codes that represent the basic operations that the computer can perform, which includes adding, moving, or comparing numbers. Because every computer use different architecture for processing so computer have there own instructions so we can say every computer have there own assembly language. It is way higher level language then machine language so its more faster and but still its hard to write and read. To run a program written using assembly language we need to convert it to machine language which is binary . This conversion is done by a program called an assembler.</li>
        <li></li>
        <li><b>Languages Examples</b></li>
        <li>x86 Assembly: Commonly used in Intel-based systems, x86 assembly is widely employed for low-level system programming and device drivers.</li>
        <li>ARM Assembly: Popular in embedded systems, mobile devices, and IoT applications, <a isInlineLink="true" href="https://www.geeksforgeeks.org/arm-processor-and-its-features/">ARM</a>assembly language is known for its power efficiency and versatility.</li>
        <li>Machine Languages: While machine languages vary between different CPU architectures, they all share the common attribute of consisting of binary code that the CPU can execute directly.</li>
        <li>Uses of Low-Level Language  </li>
        <li>Low-level programming languages find applications in various fields, including:</li>
        <li>Operating System Development: We know that a operating system needs a lot of hardware resources to operate and they must be connected each other in some way. Low level programming languages helps managing hardware resources and allow s using them with control and efficiency.</li>
        <li>Embedded Systems: In devices where hardware has to operate directly with on code, like <a isInlineLink="true" href="https://www.geeksforgeeks.org/microcontroller-and-its-types/">microcontrollers</a>, medical equipment, automotive systems, and <a isInlineLink="true" href="https://www.geeksforgeeks.org/communication-models-in-iot-internet-of-things/">IoT</a> devices, low level languages allows us to establish some control over hardware.</li>
        <li>Device Drivers: Most of the device drivers such as <a isInlineLink="true" href="https://www.geeksforgeeks.org/what-are-headphones/">headphone</a> drivers, speaker drivers are written in low level languages to ensure proper use of hardware, thus facilitating communication between hardware and operating system.</li>
        <li>Real-time Systems: There are systems which require performing actions according to time, means require strict timing and minimal response latency for example in aviation control systems and robotics, rely on low-level languages for precise control.</li>
        <li>Reverse Engineering: <a isInlineLink="true" href="https://www.geeksforgeeks.org/software-testing-basics/">Testing</a>and debugging of hardware and software. Low-level languages allow programmers to directly manipulate the registers and memory of the computer and monitor the execution of instructions. Low-level languages are invaluable for analyzing and understanding the proper functioning of software or <a isInlineLink="true" href="https://www.geeksforgeeks.org/malware-and-its-types/">malware</a>.</li>
        <li>Advantages of Low-Level Languages  </li>
        <li>Low level languages provides efficiency to programmers because they allow them to write highly optimised code which can use system resources such as memory, handling CPU cycles very efficiently</li>
        <li>Programmers are able manipulate hardware registers and memory locations, enabling precise control over devices, <a isInlineLink="true" href="https://www.geeksforgeeks.org/peripherals-devices-in-computer-organization/">peripherals</a>, and system resources using low level languages</li>
        <li>Low level languages lack abstraction means there is very less layers between programmer and hardware which allows programmers to change their code for specific tasks and gain a deep understanding of how the hardware functioning.</li>
        <li>Due to direct hardware control of low level languages, they can be used to implement security features and access control mechanisms at a very low level.</li>
        <li>Disadvantages of Low-Level Languages  </li>
        <li>Writing code in low level languages can be lot harder as compared to high level languages because in these we have to manage <a isInlineLink="true" href="https://www.geeksforgeeks.org/difference-between-register-and-memory/">memory and registers</a> at real time.</li>
        <li>There are low abstraction in low level languages they lack high level abstractions which make programming more accessible and user-friendly.</li>
        <li>Code written in low-level languages is often tightly coupled to a specific <a isInlineLink="true" href="https://www.geeksforgeeks.org/hardware-architecture-parallel-computing/">hardware architecture</a>, that’s why it cannot be used for other platforms devices.</li>
        <li>Its take a lot of time for developing a software using low level language because we need to give attention to very small details during this process.</li>
        <li>Técnicas de Direccionamiento</li>
        <li>The address field or fields in a typical instruction format are relatively small. We would like to be able to reference a large range of locations in main memory or, for some systems, virtual memory. To achieve this objective, a variety of addressing techniques has been employed. They all involve some ­rade-​­ t off between address range and/or addressing flexibility, on the one hand, and the number of memory references in the instruction and/or the complexity of address calculation, on the other. In this section, we examine the most common addressing techniques, or modes:</li>
        <li>1. <b>Immediate Mode</b>: In immediate mode, the operand itself is specified directly within the instruction. This means that the data to be operated on is given explicitly in the instruction. For example, in the instruction <q>ADD R1, #5</q>, the value <q>5</q> is directly provided in the instruction to be added to the contents of register <q>R1</q></li>
        <li>2. <b>Direct Mode</b>: Direct addressing, also known as absolute addressing, involves specifying the memory address directly within the instruction to access the operand. The CPU directly accesses the data stored at that memory address. For instance, in the instruction <q>LOAD R1, 1000</q>, the value stored at memory address <q>1000</q> is loaded into register <q>R1</q>.</li>
        <li>3. <b>Indirect Mode</b>: Indirect addressing involves specifying a memory address in the instruction, but instead of directly accessing the data at that address, the CPU retrieves the memory address from that location and then accesses the data from the retrieved address. For example, in the instruction <q>LOAD R1, (R2)</q>, the CPU loads the value from the memory address stored in register <q>R2</q> into register <q>R1</q>.</li>
        <li>4 . <b>Register addressing: </b>is similar to direct addressing. The only difference is that the address field refers to a register rather than a main memory address, basically the operand of the instruction is in the register specified:</li>
        <li>5. <b>Register Indirect Mode</b>: Register indirect addressing involves specifying a register in the instruction, and the CPU accesses the memory location whose address is contained within that register. For instance, in the instruction <q>LOAD R1, (R2)</q>, the CPU accesses the memory location whose address is stored in register <q>R2</q> and loads the data from that location into register <q>R1</q>.</li>
        <li>6. <b>Displacement Mode </b>: Displacement addressing involves adding a constant offset to a base register&#39;s value to calculate the effective address of the operand. The offset is often specified as part of the instruction or contained in a register. This mode is useful for accessing elements of arrays or data structures. For example, in the instruction <q>LOAD R1, 100(R2)</q>, the CPU loads the value from the memory address obtained by adding <q>100</q> to the contents of register <q>R2</q> into register <q>R1</q>.</li>
        <li>Relative addressing</li>
        <li>­Base-​­register addressing</li>
        <li>Indexing</li>
        <li>7. <b>Stack Mode (OR IMPLICIT)</b>: Stack addressing involves implicitly using a special-purpose register, typically called the stack pointer (SP), to access operands from the top of the stack. Operations like push and pop are used to add data onto and remove data from the stack, respectively. This mode is commonly used for function calls, local variable storage, and managing program control flow.</li>
        <li>These addressing modes provide flexibility in accessing operands and are utilized based on the requirements of specific instructions and programming paradigms. Understanding them is essential for efficient assembly language programming and computer architecture design.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2Fh6923wqhD2S_2GsBcj9Rfk2K5Y8TdjpkCNNPoBlxyyy28Ddc7I5ZRbYiOt54EkG-AnMuxfEk7M4TTQ830Mu_Q9HAAjL0iM7PR2Qn_OuEzC-0T9iqS33KVWxUmHL8Vn78.png" width="789" height="801"/></li>
        <li><b>Immediate Mode</b>:</li>
        <li>In immediate mode, the operand itself is specified directly within the instruction. This means that the data to be operated on is given explicitly in the instruction. For example, in the instruction <q>ADD R1, #5</q>, the value <q>5</q> is directly provided in the instruction to be added to the contents of register <q>R1</q></li>
        <li></li>
        <li></li>
        <li><b>Direct Addressing</b></li>
        <li>A very simple form of addressing is direct addressing, in which the address field contains the effective address of the operand:</li>
        <li>EA = A</li>
        <li>The technique was common in earlier generations of computers but is not com- mon on contemporary architectures. It requires only one memory reference and no special calculation. The obvious limitation is that it provides only a limited addressspace.</li>
        <li></li>
        <li><b>Indirect Addressing</b></li>
        <li>With direct addressing, the length of the address field is usually less than the word length, thus limiting the address range. One solution is to have the address field refer to the address of a word in memory, which in turn contains a ­full-length address of the operand. This is known as indirect addressing:</li>
        <li>As defined earlier, the parentheses are to be interpreted as meaning contents of. The obvious advantage of this approach is that for a word length of N, an addressspace of 2N is now available (básicamente si cada palabra dentro de un espacio de memoria que vos podés referenciar tiene una longitud de 8 bits, puedes referenciar 2pow8). The disadvantage is that instruction execution requires two memory references to fetch the operand: one to get its address and a second toget its value.</li>
        <li>Supongamos que tienes 4 bits, solamente puedes referenciar 16 palabras</li>
        <li>Ahora si utilizas indirect addressing y cada palabra tiene 8 bits, si referencias a una palabra, esta puede tener un span de hasta 2pow8 = 256 palabras:</li>
        <li></li>
        <li></li>
        <li><b>Register addressing:</b></li>
        <li>is similar to direct addressing. The only difference is that the address field refers to a register rather than a main memory address, basically the operand of the instruction is in the register specified:</li>
        <li></li>
        <li></li>
        <li><b>Register Indirect Mode</b>:</li>
        <li>You point to a register, and the address you look for is within that register. Is like indirect addressing but instead of pointing to a word in memory, you point to a register.</li>
        <li></li>
        <li><u><i><b>Relativa o displacement:</b></i></u></li>
        <li>Displacement addressing requires that the instruction have two address fields, at least one of which is explicit. The value contained in one address field (value = A) is used directly. The other address field, or an implicit reference based on opcode, refers to a register whose contents are added to A to produce the effective address.</li>
        <li>EA = A + (R)</li>
        <li>If you have 5 in the register and 7 in the instruction, the address would be 12.</li>
        <li><u><i>Por base o desplazamiento:</i></u>
            <ul>
                <li>La instrucción de dirección contendrá el <i><b>desplazamiento </b></i>que se sumará al <b>registro base </b>previamente asignado</li>
            </ul>
        </li>
        <li><u><i>Por referencia al programa:</i></u>
            <ul>
                <li>El <b>registro base </b>en este caso es el contador de programa, que se sumará al desplazamiento dado por instrucción</li>
            </ul>
        </li>
        <li><u><i>Por paginación o yuxtaposición:</i></u>
            <ul>
                <li>Se divide la memoria de tal forma que pueda segmentarla en distintas páginas, por lo tanto para cada programa tendré distintas páginas. Cada que quiera direccionar solamente deberé hacer referencia a la página y el desplazamiento en base a esa página (5,10 sería página 5 posición 10 en base a esa página)</li>
            </ul>
        </li>
        <li></li>
        <li></li>
        <li><u><b>Indexado</b></u></li>
        <li>Sirve para acceder a elementos dentro de un arreglo. Se suma a un número base pasado por instrucción, valores que aumentan de forma constante. Entras en el número de memoria 100, y vas aumentando 8 bits (byte), de forma constante, de esa manera puedes acceder a cada palabra dentro del arreglo.</li>
        <li></li>
        <li>Memorias</li>
        <li>Things to take into account:
</li>
        <li>Faster access time, greater cost per bit;</li>
        <li>Greater capacity, smaller cost per bit;</li>
        <li>Greater capacity, slower access time.</li>
        <li>1. <b>Memory</b>: In computer architecture, memory refers to the physical devices used to store data and instructions for processing by the CPU (Central Processing Unit) and other components of the computer. It is essential for the computer to function because it holds the programs and data that are currently being used.</li>
        <li>2. <b>Bits and Bytes</b>:
            <ul>
                <li><b>Bit</b>: Short for binary digit, a bit is the smallest unit of data in a computer. It can hold one of two values: 0 or 1. It represents the most fundamental piece of information in computing.</li>
                <li><b>Byte</b>: A byte is a group of 8 bits. Bytes are the basic units of storage in computer memory. They are used to represent characters, numbers, and other data types. For example, the letter &#39;A&#39; might be represented by the byte 01000001.</li>
            </ul>
        </li>
        <li>3. <b>Memory Units</b>:
            <ul>
                <li><b>Kilobyte (KB)</b>: Approximately 1,024 bytes.</li>
                <li><b>Megabyte (MB)</b>: Approximately 1,024 KB or 1,048,576 bytes.</li>
                <li><b>Gigabyte (GB)</b>: Approximately 1,024 MB or 1,073,741,824 bytes.</li>
                <li><b>Terabyte (TB)</b>: Approximately 1,024 GB or 1,099,511,627,776 bytes.</li>
                <li><b>Petabyte (PB)</b>: Approximately 1,024 TB or 1,125,899,906,842,624 bytes.</li>
                <li><b>Exabyte (EB)</b>: Approximately 1,024 PB or 1,152,921,504,606,846,976 bytes.</li>
            </ul>
        </li>
        <li>4. <b>Memory Types</b>:
            <ul>
                <li><b>RAM (Random Access Memory)</b>: RAM is volatile memory used by the computer to store data that is being actively used or processed. It allows for quick access to data by the CPU. However, its contents are lost when the computer is turned off.</li>
                <li><b>ROM (Read-Only Memory)</b>: ROM is non-volatile memory that retains its contents even when the computer is powered off. It typically contains firmware or low-level software instructions that are essential for booting up the computer and initializing hardware.</li>
                <li><b>Cache Memory</b>: Cache memory is a small, high-speed memory located between the CPU and main memory (RAM). It stores frequently accessed data and instructions to reduce the time it takes for the CPU to access them.</li>
                <li><b>Virtual Memory</b>: Virtual memory is a memory management technique that uses a portion of the computer&#39;s hard drive as an extension of RAM. It allows the computer to run programs that require more memory than is physically available.</li>
            </ul>
        </li>
        <li>Understanding memory, bits, and bytes is fundamental to understanding how computers store and process information. These concepts form the basis of computer architecture and are essential for both hardware and software development.</li>
        <li>Palabra</li>
        <li>No hay una definición universal del término palabra. En general, una palabra es un conjunto ordenado de bytes o bits que es la unidad normal con la que se almacena, transmite, u opera la información dentro de un determinado computador. Normalmente, si un computador tiene un juego de instrucciones de longitud fija, la longitud de las instrucciones es igual a la de la palabra.</li>
        <li>1. <b>Word</b>:
            <ul>
                <li>In computer architecture, a word is the natural unit of data used by a particular processor design. It represents the maximum size of data that the CPU can process in one operation.</li>
                <li>The size of a word can vary depending on the architecture of the processor. Common word sizes include 8, 16, 32, and 64 bits. For example, in a 32-bit architecture, the word size is 32 bits, and in a 64-bit architecture, the word size is 64 bits.</li>
                <li>The size of a word often determines the maximum amount of memory that the processor can address directly. For instance, a 32-bit processor can address up to 2^32 (approximately 4.3 billion) memory locations.</li>
            </ul>
        </li>
        <li>2. <b>Addressable Unit</b>:
            <ul>
                <li>The addressable unit is the smallest unit of memory that can be individually accessed or addressed by the CPU.</li>
                <li>In most modern computer architectures, the smallest addressable unit is typically a byte. This means that each memory location in the computer&#39;s memory is assigned a unique address, and each address corresponds to a byte of data. This is explained later with multiplexers</li>
                <li>For example, if a computer has 4 GB (gigabytes) of RAM and uses byte-addressable memory, it means there are approximately 4 billion memory locations, each corresponding to one byte of data.</li>
            </ul>
        </li>
        <li>So, to summarize, a word is the natural unit of data used by the CPU for processing, while a byte is the smallest addressable unit of memory, with each memory location in the computer&#39;s memory being uniquely identified by its address.</li>
        <li></li>
        <li><b>Design Constraints on Memory</b>:
            <ul>
                <li>Three fundamental questions: How much? How fast? How expensive?</li>
            </ul>
        </li>
        <li><b>How Much</b>:
            <ul>
                <li>Capacity is essential; applications will adapt to available capacity.</li>
            </ul>
        </li>
        <li><b>How Fast</b>:
            <ul>
                <li>Memory must keep pace with the processor to avoid performance bottlenecks.</li>
            </ul>
        </li>
        <li><b>How Expensive</b>:
            <ul>
                <li>Memory cost must be reasonable compared to other system components.</li>
            </ul>
        </li>
        <li><b>Trade-offs in Memory Design</b>:
            <ul>
                <li>Capacity, access time, and cost are interconnected.</li>
            </ul>
        </li>
        <li><b>Relationships Across Memory Technologies</b>:
            <ul>
                <li>Faster access time comes with a higher cost per bit.</li>
                <li>Greater capacity often correlates with a smaller cost per bit.</li>
                <li>However, greater capacity tends to lead to slower access times.</li>
            </ul>
        </li>
        <li><b>Design Dilemma</b>:
            <ul>
                <li>Balance between needing large-capacity, low-cost memory and high-performance, expensive, low-capacity memory.</li>
            </ul>
        </li>
        <li><b>Solution: Memory Hierarchy</b>:
            <ul>
                <li>Employing a hierarchy of memory types.</li>
            </ul>
        </li>
        <li><b>Memory Hierarchy</b>:
            <ul>
                <li>Smaller, expensive, faster memories at the top; larger, cheaper, slower memories at the bottom.</li>
            </ul>
        </li>
        <li><b>Hierarchy Characteristics</b>:
            <ul>
                <li>Decreasing cost per bit.</li>
                <li>Increasing capacity.</li>
                <li>Increasing access time.</li>
                <li>Decreasing frequency of access by the processor.</li>
            </ul>
        </li>
        <li><b>Explanation</b>:</li>
        <li>The text outlines the core considerations in memory design: capacity, access time, and cost.</li>
        <li>It discusses trade-offs among these factors and the necessity of a memory hierarchy to balance performance and cost effectively.</li>
        <li>The hierarchy ensures that the system has access to both fast, expensive memory for performance-critical tasks and larger, cheaper memory for storing larger amounts of data.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FhtEXn0im5e8JWW4y2IgCHiyx2uEWuKNriXaSTtQePooprRLwXphgGZUlzw5-01-FIQnvdW2zR2poZ1RWoYadPUjsVvhBRq3VUid-2UQT7hcjwVRcUiqVpyEUtCkGFl_f.png" width="790" height="715.9375"/></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FBTFYjNKmgvUs6OU44QHkwuO7_t8JVeaUmHkvyXkdHKVW-gaxbRMYN8Xs89zlPsMdOAM245ga5C_RhlcSFhgPRvHyptWxRmVQDWrhsXwZbdfxGYyeN980FzouB5EtDfY7.png" width="790" height="704"/></li>
        <li>1. Registers</li>
        <li>Registers are small, high-speed memory units located in the CPU. They are used to store the most frequently used data and instructions. Registers have the fastest access time and the smallest storage capacity, typically ranging from 16 to 64 bits.</li>
        <li>2. Cache Memory</li>
        <li>Cache memory is a small, fast memory unit located close to the CPU. It stores frequently used data and instructions that have been recently accessed from the main memory. Cache memory is designed to minimize the time it takes to access data by providing the CPU with quick access to frequently used data.</li>
        <li>3. Main Memory</li>
        <li>Main memory, also known as RAM (Random Access Memory), is the primary memory of a computer system. It has a larger storage capacity than cache memory, but it is slower. Main memory is used to store data and instructions that are currently in use by the CPU.</li>
        <li>Types of Main Memory</li>
        <li>Static RAM: Static RAM stores the binary information in flip flops and information remains valid until power is supplied. It has a faster access time and is used in implementing cache memory.</li>
        <li>Dynamic RAM: It stores the binary information as a charge on the capacitor. It requires refreshing circuitry to maintain the charge on the capacitors after a few milliseconds. It contains more memory cells per unit area as compared to SRAM.</li>
        <li></li>
        <li>4. Secondary Storage</li>
        <li>Secondary storage, such as hard disk drives (HDD) and solid-state drives (SSD), is a non-volatile memory unit that has a larger storage capacity than main memory. It is used to store data and instructions that are not currently in use by the CPU. Secondary storage has the slowest access time and is typically the least expensive type of memory in the memory hierarchy.</li>
        <li>5. Magnetic Disk</li>
        <li>Magnetic Disks are simply circular plates that are fabricated with either a metal or a plastic or a magnetized material. The Magnetic disks work at a high speed inside the computer and these are frequently used.</li>
        <li>6. Magnetic Tape</li>
        <li>Magnetic Tape is simply a magnetic recording device that is covered with a plastic film. It is generally used for the backup of data. In the case of a magnetic tape, the access time for a computer is a little slower and therefore, it requires some amount of time for accessing the strip.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2F2WIyZlDXGXRSzIcKxn-MFmMtW9X0nCahwRA5Yuh1BhITE7aRu2h4SM71I_JDSMubL4Jr6QFNFK-Q6tAgAk61Uophmp9mVckuKvYTuKHH7zkdq4V5Pt-jGBviZiFjNCuK.png" width="790" height="371.3"/></li>
        <li></li>
        <li></li>
        <li>Entrada y Salida</li>
        <li><b>Input/Output (I/O)</b>: This section introduces the concept of Input/Output in computer systems, emphasizing its importance in facilitating communication between the computer and external devices. It discusses the role of I/O in enabling users to interact with computers and for computers to communicate with peripherals like keyboards, mice, printers, and storage devices.</li>
        <li>What is an I/O module?</li>
        <li>An I/O (Input/Output) module is a component within a computer system responsible for managing communication between the CPU (central processing unit) and peripheral devices. It serves as an interface that enables the CPU to interact with external devices such as keyboards, mice, monitors, printers, storage devices, and network adapters. The I/O module contains logic circuits that facilitate data transfer between the CPU and peripherals, translating commands from the CPU into signals that can be understood by the connected devices, and vice versa. Additionally, I/O modules often provide buffering and error-handling mechanisms to ensure reliable data transmission between the CPU and peripherals. Overall, I/O modules play a crucial role in enabling the computer system to interact with its external environment, facilitating input and output operations essential for performing tasks and running applications.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FQgmuNfw-cGqq_iIhrXzTIAUDVXwIwudzBPwEHjS8a4tcblB03UDeICtACNFaEwOL8kxbe5aTsvbFEERSzCHPDFGvWVZBIAXMGQoSRejcAkZvUOR4nhQqZI1RnIdhaQWY.png" width="575" height="515"/></li>
        <li></li>
        <li>Overview of I/O Operations:  
            <ul>
                <li>In a computer system, I/O operations involve using various external devices to exchange data between the computer and the external environment.</li>
                <li>These external devices connect to the computer via links to I/O modules, facilitating the exchange of control signals, status updates, and data.</li>
                <li>External devices connected to I/O modules are commonly referred to as peripheral devices or peripherals.</li>
                <li></li>
            </ul>
        </li>
        <li>External Devices: </li>
        <li>Here, various types of external devices are explored, ranging from simple devices like keyboards and mice to more complex peripherals such as printers, scanners, and storage devices like hard drives and solid-state drives (SSDs). The section may also discuss the characteristics and interfaces of different external devices.</li>
        <li></li>
        <li><u><b>Classification of External Devices: </b></u> </li>
        <li>External devices can be broadly categorized into three types:
            <ul>
                <li>1. <b>Human Readable</b>: Devices designed for communication with the computer user, such as monitors, keyboards, and touchscreens.
                    <ul>
                        <li>These devices are designed for humans to interact with the computer, like video display terminals (VDTs) and printers. They display information in a format that people can easily understand.</li>
                    </ul>
                </li>
                <li>2. <b>Machine Readable</b>: Devices intended for communication with equipment, such as barcode scanners, sensors, and actuators.
                    <ul>
                        <li>These devices are meant to communicate with other machines or equipment. Examples include magnetic disk and tape systems, as well as sensors and actuators used in robotics. They usually process data in a format that&#39;s suitable for machines.</li>
                    </ul>
                </li>
                <li>3. <b>Communication</b>: Devices suitable for communicating with remote devices, such as modems, network adapters, and wireless transceivers.
                    <ul>
                        <li>These devices facilitate communication between the computer and remote devices. They enable data exchange over long distances. Examples could be modems or network adapters.</li>
                    </ul>
                </li>
            </ul>
        </li>
        <li></li>
        <li>In simple terms, input/output (I/O) operations involve using various external devices to exchange data between a computer and the outside world. These devices connect to the computer through an I/O module, which serves as the link for transferring control signals, status updates, and actual data between the device and the computer.</li>
        <li>For instance, when you type on a keyboard, the keyboard is a human-readable device. The data you input is sent to the computer through the I/O module. Similarly, when a computer sends a print job to a printer, the printer is a human-readable device, and the data is sent through the I/O module.</li>
        <li>It&#39;s important to note that while devices like disk and tape systems are often considered part of the computer&#39;s memory hierarchy, they are controlled by I/O modules for data transfer, which is why they are discussed in this chapter focusing on I/O operations.</li>
        <li>When a computer wants to use a device, it sends control signals to tell the device what to do, like sending data or receiving it. The device then does its job with the help of control logic. For example, a disk drive might move its reading head to a specific position based on instructions from the computer.</li>
        <li>Data is sent between the device and the computer in the form of bits (0s and 1s), and the device might need to convert this electrical data into other types of energy (like sound or movement) or vice versa.</li>
        <li>To manage this data transfer smoothly, there&#39;s usually a buffer associated with the device. This buffer temporarily holds data as it moves between the device and the computer. Buffers can vary in size depending on the type of device. For instance, simple devices like keyboards might have small buffers, while complex ones like disk drives might have much larger ones.</li>
        <li></li>
        <li>Useful definitions
            <ul>
                <li>1. <b>Communication devices</b>: These are devices that enable a computer to send and receive data to and from other devices, which could be anything from a keyboard or a printer to another computer.</li>
                <li>2. <b>Control signals</b>: These signals determine what action a device will perform, like sending data to the computer (INPUT or READ), receiving data from the computer (OUTPUT or WRITE), indicating its current status, or performing specific functions (like positioning a disk head in a disk drive).</li>
                <li>3. <b>Data signals</b>: This refers to the actual information being sent to or received from the computer, usually in the form of binary digits (bits).</li>
                <li>4. <b>Status signals</b>: These signals indicate the current state of the device, such as whether it&#39;s ready to transfer data or not.</li>
                <li>5. <b>Control logic</b>: This is the part of the device that controls its operation based on instructions received from the computer. It ensures that the device performs the necessary tasks according to the commands it receives.</li>
                <li>6. <b>Transducer</b>: This component converts data between different forms of energy, for example, converting electrical signals to physical movement (like positioning a disk head) or vice versa.</li>
                <li>7. <b>Buffer</b>: A buffer is a temporary storage area that holds data being transferred between the device and the computer. It helps manage the flow of data, especially when there might be differences in speed between the two.</li>
                <li>8. <b>Interface</b>: This is the connection point between the device and the computer, allowing them to communicate with each other.</li>
                <li></li>
                <li></li>
            </ul>
        </li>
        <li>Keyboard Example  </li>
        <li>The most common way for users to interact with computers is through a keyboard and monitor setup.</li>
        <li>Users input data through the keyboard, which is then transmitted to the computer and may also be displayed on the monitor.</li>
        <li>The monitor also displays data provided by the computer.</li>
        <li>Characters are the basic units of exchange, each associated with a code typically 7 or 8 bits long, with the International Reference Alphabet (IRA) being a commonly used text code.</li>
        <li>IRA uses 7-bit binary codes, allowing for the representation of 128 different characters.</li>
        <li>Characters are classified into printable and control characters, with printable characters being those that can be printed or displayed on a screen, and control characters used for controlling printing/displaying or communications procedures.</li>
        <li>When a key is pressed on the keyboard, it generates an electronic signal interpreted by the keyboard&#39;s transducer and translated into the corresponding IRA code bit pattern.</li>
        <li>This pattern is then transmitted to the computer&#39;s I/O module for processing and storage.</li>
        <li>On output, IRA code characters are transmitted from the computer to external devices via the I/O module.</li>
        <li>The transducer at the device interprets the code and sends the necessary electronic signals to display the character or perform the requested control function.</li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FWFFB2o896B7QuoE690Acc74BLmWVkda7UtKVrbFpmnunzZ4PFMh4sXmNp9IQDPygBG78B1xh9ylWB4kkOSeVh_omWq-rEur3UdEq53krOi9Li_6wYHxGZ5z9rpuv5Mz1.png" width="558" height="450"/></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li>I/O Modules:</li>
        <li>This section covers the hardware components responsible for managing I/O operations, known as I/O modules. It explains their role in controlling data transfer between the CPU and external devices, including handling data formatting, error detection, and device control.</li>
        <li>The major functions or requirements for an I/O module fall into the following categories:</li>
        <li>Control and timing</li>
        <li>Processor communication</li>
        <li>Device communication</li>
        <li>Data buffering</li>
        <li>Error detection</li>
        <li>During any period of time, the processor may communicate with one or more external devices in unpredictable patterns, depending on the program’s need for I/O. The internal resources, such as main memory and the system bus, must be shared among a number of activities, including data I/O. Thus, the I/O function includes a control and timing requirement, to coordinate the flow of traffic between internal resources and external devices. For example, the control of the transfer of data from an external device to the processor might involve the following sequence of steps:</li>
        <li>The processor interrogates the I/O module to check the status of the attached device.</li>
        <li>The I/O module returns the device status.</li>
        <li>If the device is operational and ready to transmit, the processor requests the transfer of data, by means of a command to the I/O module.</li>
        <li>The I/O module obtains a unit of data (e.g., 8 or 16 bits) from the external device.</li>
        <li>The data are transferred from the I/O module to the processor.</li>
        <li>The I/O module plays a crucial role in communication between the processor and external devices. Processor communication involves:</li>
        <li>Command decoding: Commands from the processor are interpreted by the I/O module, often transmitted via the control bus. For instance, commands for a disk drive might include operations like READ SECTOR or WRITE SECTOR, each possibly carrying parameters sent over the data bus.</li>
        <li>Data exchange: Data moves between the processor and the I/O module via the data bus.</li>
        <li>Status reporting: Given the slow nature of peripherals, it&#39;s essential to track the I/O module&#39;s status. Signals like BUSY and READY inform the processor about the module&#39;s readiness or ongoing tasks, alongside signals for error conditions.</li>
        <li>Address recognition: Similar to memory addressing, each I/O device possesses a unique address. Thus, the I/O module must identify and respond to the address corresponding to each peripheral it manages.</li>
        <li></li>
        <li>I/O Module Structure  </li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FiE-Y5BUq4OM9RvMASJQBPVfgH8o6aV6gWm7rIDTL_xpePW7CbJbqW8-V21ZcQGRGjHfAD-lai77E8JmoMhd3oufEjzSXb9h7o_iyRWMQGm8wCKTId-OI5pIyF6dGz8V5.png" width="790" height="446.35"/></li>
        <li></li>
        <li></li>
        <li>I/O techniques</li>
        <li>Programmed I/O (PIO)</li>
        <li>Direct Memory Access (DMA):</li>
        <li>Interrupt-Driven I/O:</li>
        <li></li>
        <li>Programmed I/O: </li>
        <li>When the processor executes a program and encounters an instruction related to I/O, it issues a command to the appropriate I/O module. With programmed I/O, the module performs the requested action and sets the corresponding bits in the I/O status register. However, it does not further engage with the processor, including interrupting it. Thus, the processor must periodically check the module&#39;s status until the operation is complete.</li>
        <li>The image that compares the 3 methods provides an example of using programmed I/O to read a block of data from a peripheral device (such as a record from tape) into memory. Data are read one word (e.g., 16 bits) at a time. For each word read, the processor must remain in a status-checking cycle until it confirms that the word is available in the I/O module&#39;s data register. This flowchart illustrates the primary drawback of this technique: it&#39;s a time-consuming process that needlessly occupies the processor.</li>
        <li></li>
        <li></li>
        <li>I/O commands  </li>
        <li>To execute an I/O-related instruction, the processor issues an address specifying the particular I/O module and external device, along with an I/O command. There are four types of I/O commands that an I/O module may receive when addressed by a processor:</li>
        <li><b>Control</b>: Used to activate a peripheral and define its action. For instance, a magnetic tape unit may be instructed to rewind or advance one record. These commands are customized for specific types of peripheral devices.</li>
        <li><b>Test</b>: Employed to check various status conditions associated with an I/O module and its peripherals. The processor ensures that the peripheral is powered on and available for operation. It also verifies if the most recent I/O operation is complete and if any errors occurred.</li>
        <li><b>Read</b>: Initiates the I/O module to retrieve data from the peripheral and store it in an internal buffer (depicted as a data register in Figure 7.3). The processor can then access the data by requesting the I/O module to place it on the data bus.</li>
        <li><b>Write</b>: Instructs the I/O module to receive data (byte or word) from the data bus and transmit it to the peripheral.</li>
        <li></li>
        <li><img src="local://%2Fhome%2Fivan%2Fremnote%2Fremnote-6569ec387720c4c49db031fb%2Ffiles%2FTI_Df9pA9ruYcnJTZsT2fbZQla5Ogt4k0-wKuFyBqemKrYM7DtFL4Atz25GH0kOhDgT6UhpiBYWeyr4YSWkCIttbTaxXxEeSwa_Ti-c6yMwe-87YRyz74hUONMzRyOWT.png" width="790" height="569.7875"/></li>
        <li></li>
        <li>1. <b>Programmed I/O (PIO)</b>:</li>
        <li>Programmed I/O is the most basic form of I/O handling. In this method, the CPU is directly responsible for transferring data between the I/O device and memory. The CPU executes specific instructions to read or write data to/from the I/O device. It involves the CPU checking the status of the I/O device, issuing commands to it, and then transferring data between memory and the device.</li>
        <li>Advantages:
            <ul>
                <li>Simple implementation.</li>
                <li>Suitable for transferring small amounts of data or when the frequency of I/O operations is low.</li>
            </ul>
        </li>
        <li>Disadvantages:
            <ul>
                <li>Inefficient for transferring large amounts of data due to the high overhead on the CPU.</li>
                <li>CPU is tied up during I/O operations, reducing overall system performance.</li>
            </ul>
        </li>
        <li>2. <b>Direct Memory Access (DMA)</b>:</li>
        <li>DMA is a method that allows data to be transferred directly between an I/O device and memory without involving the CPU. DMA controllers are specialized hardware units that manage these data transfers. The CPU sets up the DMA controller with information about the data transfer (source, destination, size, etc.), and then the DMA controller takes over the data movement while the CPU is free to perform other tasks.</li>
        <li>Advantages:
            <ul>
                <li>Offloads data transfer tasks from the CPU, improving overall system performance.</li>
                <li>Particularly effective for transferring large amounts of data.</li>
            </ul>
        </li>
        <li>Disadvantages:
            <ul>
                <li>Requires additional hardware (DMA controller).</li>
                <li>More complex to implement than programmed I/O.</li>
            </ul>
        </li>
        <li>3. <b>Interrupt-Driven I/O</b>:</li>
        <li>In interrupt-driven I/O, the CPU is not constantly polling the I/O device to check if it needs attention. Instead, the CPU initiates an I/O operation and then continues executing other tasks. When the I/O device needs attention (e.g., data is ready for transfer or an operation is complete), it interrupts the CPU, causing it to temporarily suspend its current task and handle the I/O request.</li>
        <li>Advantages:
            <ul>
                <li>Allows the CPU to perform other tasks while waiting for I/O operations to complete.</li>
                <li>Improves overall system responsiveness.</li>
            </ul>
        </li>
        <li>Disadvantages:
            <ul>
                <li>Requires hardware support for interrupt handling.</li>
                <li>More complex to implement than programmed I/O.</li>
            </ul>
        </li>
        <li>In summary, programmed I/O involves the CPU directly managing data transfers between memory and I/O devices, DMA offloads this task to a specialized controller to improve performance, and interrupt-driven I/O allows the CPU to multitask while handling I/O operations by responding to interrupts from devices. Each method has its advantages and is suited to different scenarios based on factors like data transfer size, frequency, and system performance requirements.</li>
        <li></li>
        <li>When to use which?</li>
        <li>1. <b>Programmed I/O (PIO)</b>:</li>
        <li><b>Best for</b>:
            <ul>
                <li>Simple I/O operations with low data transfer rates and sporadic events.</li>
            </ul>
        </li>
        <li><b>Example Scenario</b>:
            <ul>
                <li>Reading input from a single button on a microcontroller-based device. The device only needs to check the status of the button occasionally, and the data transfer involves only a single bit. Using programmed I/O, the microcontroller can periodically check the state of the button by reading a specific memory address or I/O port associated with the button input.</li>
            </ul>
        </li>
        <li>2. <b>Direct Memory Access (DMA)</b>:</li>
        <li><b>Best for</b>:
            <ul>
                <li>Large data transfers with minimal CPU involvement.</li>
            </ul>
        </li>
        <li><b>Example Scenario</b>:
            <ul>
                <li>Transferring a large file from a hard disk drive to system memory in a computer. The CPU initiates the DMA transfer by providing the DMA controller with the source (disk) and destination (memory) addresses and the size of the data to be transferred. The DMA controller then handles the data transfer directly between the disk and memory, allowing the CPU to perform other tasks simultaneously without being tied up by the data transfer process.</li>
            </ul>
        </li>
        <li>3. <b>Interrupt-Driven I/O</b>:</li>
        <li><b>Best for</b>:
            <ul>
                <li>Systems requiring prompt response to external events.</li>
            </ul>
        </li>
        <li><b>Example Scenario</b>:
            <ul>
                <li>Network communication in a server. When data packets arrive from the network interface card, they trigger interrupts, prompting the CPU to handle the incoming data immediately. This allows the system to respond quickly to incoming network requests without continuously polling the network interface.</li>
            </ul>
        </li>
        <li><b>Example with  keyboard and mouse</b></li>
        <li>1. <b>Keyboard</b>:
            <ul>
                <li>Keyboards generate input events (keystrokes) sporadically and intermittently.</li>
                <li>Each keystroke needs to be processed promptly to maintain smooth user interaction.</li>
                <li>Using interrupt-driven I/O, the keyboard can interrupt the CPU whenever a key is pressed or released, ensuring immediate processing of each keystroke without the need for constant polling by the CPU.</li>
                <li>This method allows the CPU to remain responsive to other tasks while still handling keyboard input efficiently.</li>
            </ul>
        </li>
        <li>2. <b>Mouse</b>:
            <ul>
                <li>Similar to keyboards, mice also generate input events (movements and clicks) sporadically.</li>
                <li>Mouse input requires immediate response for accurate cursor movement and interaction with graphical elements.</li>
                <li>Interrupt-driven I/O allows the mouse to interrupt the CPU whenever movement or button clicks occur, ensuring that the mouse input is processed promptly and accurately.</li>
                <li>This method enables smooth and responsive cursor movement without requiring continuous CPU polling.</li>
            </ul>
        </li>
        <li>8. <b>I/O Channels and Processors</b>: I/O channels and processors are specialized units dedicated to handling I/O operations efficiently. This section discusses their architecture, functions, and how they collaborate with the CPU and other system components to manage I/O.</li>
        <li>9. <b>External Interconnection Standards</b>: This part covers the standards and protocols used for connecting external devices to computers, such as USB, Thunderbolt, SATA, and Ethernet. It explains their features, compatibility, and typical usage scenarios.</li>
        <li>10. <b>IBM zEnterprise EC12 I/O Structure</b>: This case study provides insights into the I/O architecture of the IBM zEnterprise EC12 mainframe system. It may discuss its unique features, scalability, and how it handles I/O operations in large-scale computing environments.</li>
        <li>11. <b>Key Terms, Review Questions, and Problems</b>: This section summarizes the key terms introduced in the chapter, provides review questions to test understanding, and presents problems to reinforce concepts through practical application.</li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li>Preguntas de la guía 1</li>
        <li>1. <b>¿Qué es una computadora?</b>
            <ul>
                <li>Una computadora es un dispositivo electrónico diseñado para procesar datos de manera automática mediante la ejecución de programas. Sus componentes fundamentales son:</li>
                <li><b>CPU (Unidad Central de Procesamiento)</b>: Realiza las operaciones de cálculo y control en la computadora.</li>
                <li><b>Memoria principal</b>: Almacena temporalmente datos e instrucciones que el CPU necesita para procesar.</li>
                <li><b>Dispositivos de entrada</b>: Permiten al usuario ingresar datos a la computadora (como teclado, ratón, etc.).</li>
                <li><b>Dispositivos de salida</b>: Muestran resultados o información procesada por la computadora (como pantalla, impresora, etc.).</li>
                <li><b>Dispositivos de almacenamiento</b>: Guardan datos a largo plazo (como discos duros, unidades de estado sólido, etc.).</li>
            </ul>
        </li>
        <li>2. <b>¿Qué es el CPU?</b>
            <ul>
                <li>El CPU (Unidad Central de Procesamiento) es el componente principal de una computadora, encargado de ejecutar las instrucciones de los programas y realizar operaciones aritméticas y lógicas. Está compuesto por la unidad de control, que coordina las operaciones, y la unidad aritmético-lógica, que realiza cálculos y operaciones lógicas.</li>
            </ul>
        </li>
        <li>3. <b>¿A qué se llama memoria principal? ¿Cuál es su función? Ejemplifique.</b>
            <ul>
                <li>La memoria principal es un tipo de almacenamiento temporal de acceso rápido donde se almacenan datos y programas que están en uso activo por el CPU. Su función principal es proporcionar un espacio de trabajo para el procesador, permitiéndole acceder rápidamente a los datos que necesita para ejecutar instrucciones. Ejemplo: la RAM (Memoria de Acceso Aleatorio) es un tipo de memoria principal donde se cargan los programas y datos que se están utilizando en un momento dado.</li>
            </ul>
        </li>
        <li>4. <b>¿A qué se llama memoria secundaria? ¿Cuál es su función? Ejemplifique.</b>
            <ul>
                <li>La memoria secundaria es un tipo de almacenamiento de acceso más lento pero de mayor capacidad que la memoria principal. Su función principal es almacenar datos de manera permanente, incluso cuando la computadora está apagada. Ejemplo: los discos duros y las unidades de estado sólido (SSD) son tipos de memoria secundaria donde se almacenan archivos y programas de manera permanente.</li>
            </ul>
        </li>
        <li>5. <b>¿A qué se llama almacenamiento fuera de línea?</b>
            <ul>
                <li>El almacenamiento fuera de línea se refiere a cualquier forma de almacenamiento que no está directamente conectada o accesible para el sistema en un momento dado. Esto puede incluir dispositivos de almacenamiento como discos duros externos, unidades flash USB o incluso servicios en la nube a los que se accede a través de internet.</li>
            </ul>
        </li>
        <li>6. <b>¿Qué es una jerarquía de memorias?</b>
            <ul>
                <li>La jerarquía de memorias es un concepto que describe la organización de diferentes niveles de almacenamiento en una computadora, cada uno con diferentes velocidades de acceso y capacidades. En general, cuanto más cerca esté un nivel de memoria del CPU, más rápido será el acceso pero menor será su capacidad, y viceversa.</li>
            </ul>
        </li>
        <li>7. <b>Defina el concepto de memoria caché.</b>
            <ul>
                <li>La memoria caché es un tipo de memoria de acceso rápido y tamaño reducido que se encuentra entre el CPU y la memoria principal en la jerarquía de memorias. Su función principal es almacenar temporalmente datos e instrucciones que el CPU necesita acceder con frecuencia, reduciendo así el tiempo de acceso a la memoria principal y mejorando el rendimiento del sistema. La memoria caché opera según el principio de la localidad de referencia, que establece que los programas tienden a acceder a los mismos datos o instrucciones repetidamente en un corto período de tiempo.</li>
            </ul>
        </li>
        <li>8. <b>Defina el concepto de buffer:</b>
            <ul>
                <li>Un buffer es una región de memoria temporal utilizada para almacenar datos mientras se transfieren entre dos dispositivos o procesos con diferentes velocidades de operación. Funciona como un área de almacenamiento intermedio que permite una comunicación más eficiente entre los componentes que operan a diferentes velocidades. Por ejemplo, en la reproducción de audio o video en línea, un buffer puede almacenar fragmentos de datos anticipadamente para evitar interrupciones durante la reproducción cuando la conexión de red es lenta.</li>
            </ul>
        </li>
        <li>9. <b>¿Qué es la memoria virtual?</b>
            <ul>
                <li>La memoria virtual es una técnica que utiliza el sistema operativo para ampliar la capacidad de la memoria física de una computadora al permitir que partes de los programas y datos que no se están utilizando activamente se almacenen temporalmente en el disco duro. Esto permite que los programas utilicen más memoria de la que está físicamente disponible en la RAM. La memoria virtual se gestiona mediante un sistema de paginación o segmentación, donde se dividen los programas en fragmentos llamados páginas o segmentos, que se cargan y descargan según sea necesario.</li>
            </ul>
        </li>
        <li>10. <b>¿Cuáles son los componentes fundamentales del CPU?</b>
            <ul>
                <li>Los componentes fundamentales del CPU son:</li>
                <li>Unidad de Control (UC)</li>
                <li>Unidad Aritmético Lógica (ALU)</li>
                <li>Registros internos</li>
            </ul>
        </li>
        <li>11. <b>¿Cuál es la función de la UC (Unidad de Control)?</b>
            <ul>
                <li>La función principal de la Unidad de Control es interpretar y ejecutar las instrucciones del programa. Coordina las operaciones del CPU, controla el flujo de datos entre la CPU y otras partes del sistema, y se encarga de buscar, decodificar y ejecutar las instrucciones almacenadas en la memoria.</li>
            </ul>
        </li>
        <li>12. <b>¿Cuál es la función de la ALU (Unidad Aritmético Lógica)?</b>
            <ul>
                <li>La función principal de la ALU es realizar operaciones aritméticas (como sumas y restas) y operaciones lógicas (como AND, OR y NOT) sobre los datos que recibe del registro interno y de la memoria principal.</li>
            </ul>
        </li>
        <li>13. <b>¿Qué elemento de la UC me indica la dirección de la siguiente instrucción a ejecutarse?</b>
            <ul>
                <li>El Program Counter (Contador de Programa) es el elemento de la Unidad de Control que indica la dirección de la siguiente instrucción a ejecutarse. Es un registro que almacena la dirección de memoria de la siguiente instrucción que el CPU debe recuperar y ejecutar.</li>
            </ul>
        </li>
        <li>14. <b>¿Qué es el ciclo de vida de una instrucción y cuáles son sus fases?</b>
            <ul>
                <li>El ciclo de vida de una instrucción es el proceso que sigue una instrucción desde que se carga en el CPU hasta que se completa su ejecución. Sus fases son:</li>
                <li><b>Buscar</b>: El CPU busca la siguiente instrucción en la memoria.</li>
                <li><b>Decodificar</b>: La Unidad de Control interpreta la instrucción y determina qué acción realizar.</li>
                <li><b>Ejecutar</b>: La instrucción se ejecuta, lo que puede implicar operaciones aritméticas, lógicas o de transferencia de datos.</li>
                <li><b>Almacenar (si es necesario)</b>: Algunas instrucciones pueden requerir almacenar resultados en la memoria o en registros específicos.</li>
            </ul>
        </li>
        <li>15. <b>Explique qué son las técnicas de direccionamiento. Explique y distinga los modos directo, indirecto, inmediato y por base y desplazamiento.</b>
            <ul>
                <li>Las técnicas de direccionamiento se refieren a los métodos utilizados para especificar la dirección de los operandos en una instrucción de máquina. Los modos comunes son:</li>
                <li><b>Directo</b>: La dirección del operando se especifica directamente en la instrucción.</li>
                <li><b>Indirecto</b>: La instrucción contiene la dirección de memoria donde se encuentra la dirección del operando.</li>
                <li><b>Inmediato</b>: El operando en sí mismo se especifica directamente en la instrucción.</li>
                <li><b>Por base y desplazamiento</b>: Se suman una dirección base almacenada en un registro y un desplazamiento especificado en la instrucción para calcular la dirección del operando.</li>
            </ul>
        </li>
        <li>16. <b>¿Qué son los periféricos?</b>
            <ul>
                <li>Los periféricos son dispositivos conectados a una computadora que proporcionan funcionalidades adicionales para realizar tareas específicas de entrada, salida o almacenamiento de datos. Ejemplos comunes incluyen teclados, ratones, impresoras, escáneres, discos duros externos, etc.</li>
            </ul>
        </li>
        <li>17. <b>Explique los mecanismos para tratamiento de E/S: Guiado por programa, por interrupciones y acceso directo a memoria.</b>
            <ul>
                <li><b>Guiado por programa</b>: El CPU controla directamente el flujo de datos de entrada y salida entre la memoria y los periféricos. Este enfoque requiere una cooperación explícita del programa para realizar operaciones de E/S.</li>
                <li><b>Por interrupciones</b>: Los periféricos pueden interrumpir el flujo normal de ejecución del CPU para señalar que necesitan atención. El CPU responde a estas interrupciones ejecutando rutinas de servicio de interrupción para manejar las operaciones de E/S.</li>
                <li><b>Acceso directo a memoria (DMA)</b>: Los periféricos con capacidades DMA pueden transferir datos directamente entre sí y la memoria principal sin intervención del CPU, lo que libera al CPU para realizar otras tareas mientras se lleva a cabo la transferencia de datos.</li>
            </ul>
        </li>

    </ul>
    </body>
</html>
