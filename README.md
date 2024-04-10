# **EmbeddedSystem**


## **Introduction**

### **Embedded System**

* It is  a combination of <ins> Both Hardware and Software with some mechanical parts </ins> to perform a <ins>specific task </ins> is called Embedded System.
* mobile is not is embedded system, it is a General purpose machine.
* Example: Printer, Induction Stove , Washing Machine

### **Classification of Embedded System**

1. Realtime Embedded System 
    * System which completes the TASK within Specific Time
      * Hard real time -- Nuclear Reactor
      * soft real time -- Game Controller
2. Network Embedded System 
    * Communicate with other Embedded Systems through ethernet or local area network or some other devices like routers.
3. Mobile Embedded System 
    * which act as a standalone
    * example : pacemakers (which has to operated by battery for a long time)

### **Types of Processors and Controllers for Embedded System**

1. Microprocessors/Microcontrollers - (8085/8086/8051)
2. DSP/DSC - (TMS320C6000/TSM320C2000)
3. CPLD/FPGA - Xilinx Coolrunner /ZYNQ
4. ASIC - Intel Movidius Stick , TGAM ,
5. SOC - ESP32-S3 , TI OMAP

### **Programming Languages you can choose for Embedded system**

1. ASM
2. C
3. Mixed C/ASM
4. Python
5. HDL
6. Graphical / VISUAL

![peripherals](./Images/Peripherals.jpg)

### **List of companies Dominating processor core**

1. Intel 8051:
    * Processor Core: 8051
    * Company: Intel
    * Summary: Intel's 8051 microcontroller is known for its simplicity and versatility, making it widely used in embedded systems for diverse applications.

2. ARM:
    * Processor Cores: LPC2148, STM32 (ARM Cortex-M series)
    * Company: ARM
    * Summary: ARM, a British company, provides energy-efficient and scalable processor cores. The LPC2148 and STM32 microcontroller families utilize ARM Cortex-M cores, offering flexibility for various applications.

3. Microchip (PIC):
    * Processor Core: PIC
    * Company: Microchip Technology
    * Summary: Microchip's PIC microcontrollers are popular for their versatility and ease of integration, finding extensive use in embedded systems across different industries.

4. Tensilica - Cadence Design System (ESP32):
    * Processor Core: Tensilica Xtensa (used in ESP32)
    * Company: Cadence Design Systems
    * Summary: Tensilica, a division of Cadence, provides customizable processor cores. The Xtensa architecture, seen in the ESP32 microcontroller, allows developers to tailor performance and power characteristics to specific needs.

### **Application of ESD**

* Aerospace
* Automotive infotainment
* smart home
* industry 4.0 Automation
* Robotics
* Communication
* Audio , Video and
* Medical Imaging

### Convert an Idea to Prototype

![peripherals](./Images/Prototype.jpg)

### Embedded Development Life cycle

![EmbeddedDevelpmentLifeCycle](./Images/EmbeddedDevelopmentLifeCycle.jpg)


## **How To Choose a Right Processor**

![TypesOfProcessorsAndControllers](./Images/TypesOfProcessorsAndController.jpg)

> To Know about the manufactures of different processors and controllers you can visit [DigiLink](https://www.digikey.in/)

![ManufacturerOfProcessorsAndControllers](./Images/ManufacturesOfProcessors.jpg)

### MicroProcessor

![MicroProcessor](./Images/MicroProcessor.jpg)

* A microprocessor is a programmable integrated circuit (IC) that serves as the central processing unit (CPU) of a computer or electronic device. It is essentially the "brain" of a computer system, responsible for executing instructions and performing calculations. microprocessors require peripherals to interact with the external world and perform various tasks. Peripherals are additional devices and components that connect to the microprocessor to extend its capabilities and facilitate communication with the outside environment.
* Example : 8051

### MicroController 

![MicroController](./Images/Microcontroller.jpg)

* A microcontroller is a compact, integrated circuit (IC) that contains a processor core, memory, and programmable input/output peripherals. Unlike a general-purpose microprocessor, which is designed for tasks like running an operating system and handling a wide range of applications, a microcontroller is specifically intended for embedded systems and dedicated control applications.

### DSP (Digital Signal Processor)

* Digital Signal Processor is Mathematics on chip
* DSPs usually run applications with hard real-time constraints.
* DSPs usually process infinite continuous data streams
* MAC capability (Multiply-Accumulate operation)
* DSP Processors are Microprocessors designed for efficient mathematical manipulation of digital signals

#### why DSP Processor

* MicroControllers are control oriented , DSP are data path oriented .
* use a GPP Processor when the following are required:
  * Large Memory
  * Advanced operating system
* Use a DSP processor when the following are required:
  * Precision
  * cost saving
  * smaller size
  * low power consumption
  * processing of signals in realtime
  
> DSP processor uses Harvard architecture 

![[architecture]](./Images/architecture.jpg)


### FPGA VS CPLG

* FPGA - Field Programmable Gate Array, CPLD - Complex Programmable Logic Devices
* CPLD is control path oriented, FPGA is Data path oriented

![[CPLDarchitecture]](./Images/CPLDArchitecture.jpg)

![[FPGAarchitecture]](./Images/FPGAArchitecture.jpg)

![[Multicore]](./Images/multicore.jpg)

![[Package]](./Images/package.jpg)



## ARM

* Acorn RISC Machine -> Advanced RISC machine
* Founded in 1990
  * spun out of Acron Computers
* Designs the ARM range of RISC processor
* Licenses ARM core for Design Partners
  * ARM does not fabricate silicon on own
* Develops technology to assist with ARM Arch
  * Software Tools
  * Boards , Debug Hardware , Peripherials
  * Application software , BUs Architecture 

### why ARM

* Built in Architecture extensions
  * THUMB 2 - Greatly improved code density
  * DSP - signal process directly in the RISC core
  * jazelle - Java acceleration
  * Trustzone - Maximum security environment
* Core Performance
* Tools of Choice
* Wide Support
* Low Power Consumption

### ARM Processor VS ARM Architecture

#### ARM Architecture

* This refers to the design principles, instruction set, and specifications developed by ARM Holdings. The ARM architecture defines how instructions are executed, how data is processed, and how the processor interacts with other components in a system. It's like the blueprint or framework for building processors.
* Documented in the Architecture Reference Manual

#### ARM Processor

* An ARM processor is a specific implementation of the ARM architecture by a particular manufacturer. There are various ARM processors available from different companies like Qualcomm, Apple, Samsung, and others. Each manufacturer may customize the ARM architecture to some extent, adding their own features, optimizations, or additional instructions tailored to specific applications or performance requirements.
* Documented in the Processor Technical Reference Manual

In summary, the ARM architecture is the overarching design framework, while ARM processors are specific implementations of that architecture by different manufacturers, each with its own variations and optimizations.


### ARM Versions

<https://en.wikipedia.org/wiki/List_of_ARM_processors>

![[ARM-Versions]](./Images/ARMVersions.jpg)

* Cortex-A series (Application)
  * High performance processors capable of full Operating System (OS) support
  * Applications include smartphones, digital TV, smart books
* Cortex-R series (Real-time)
  * High performance and reliability for real-time applications;
  * Applications include automotive braking system, powertrains
* Cortex-M series (Microcontroller)
  * Cost-sensitive solutions for deterministic microcontroller applications
  * Applications include microcontrollers, smart sensors
* SecurCore series
  * High security applications
* Earlier classic processors including Arm7, Arm9, Arm

### Architecture Extensions

![[THumb]](./Images/Thumb.jpg)

#### **THUMB:**

* The original Thumb instruction set was introduced with ARMv4 architecture. It allows instructions to be encoded in a 16-bit format, which is half the size of standard 32-bit ARM instructions. This compression leads to reduced memory usage and improved code density. Thumb instructions are generally simpler and more compact than their 32-bit ARM counterparts. However, Thumb instructions sacrifice some performance compared to full ARM instructions because they typically perform fewer operations per cycle.
* introduced in ARM7TDMI Processor ("T" stands for THUMB)
* subsequently supported in every ARM processor developed since

#### **THUMB2:**

* Thumb-2, introduced with ARMv6 architecture, is an extension of the original Thumb instruction set. It retains the 16-bit encoding for most instructions but introduces a wider range of instructions and capabilities. Thumb-2 allows for a mix of both 16-bit Thumb instructions and 32-bit Thumb instructions, providing better performance and flexibility. This hybrid approach allows Thumb-2 to achieve a good balance between code size and performance, making it suitable for a wider range of applications.
* all processor operations can indeed be handled in "Thumb state".
* supported across the Cortex-M processor range

#### **TrustZone:**

* Provide a Trusted Execution Environment (TEE)
* Consistent programming model across platforms and applications.
* Hardware backed security environment

#### **JazelleⓇ:**

* Technology to enable Jazelle H/w in any existing JVM
* Full featured multi-tasking Java Virtual Machine JVM
* Enables acceleration of execution environments

#### AMBA (Advanced Microcontroller Bus Architecture):

* The AMBA (Advanced Microcontroller Bus Architecture) system is an open standard that defines how different components within a System-on-Chip (SoC) communicate with each other. It's essentially a set of rules and specifications for on-chip communication, offering several advantages: Faster Data Transfer , Efficient Design , Reduced Power Consumption.
* Multiple Bus Types: AMBA defines different bus protocols, each suited for different scenarios:
  * <ins> AHB (Advanced High-performance Bus) </ins>: High-performance for data-intensive tasks between main processors and memory controllers.
  * <ins> ASB (Advanced System Bus) </ins>: Connects high-bandwidth components like external memory interfaces. (Less common nowadays) 
  * <ins> APB (Advanced Peripheral Bus) </ins>: Low-power, low-performance bus ideal for low-bandwidth peripherals.

![[AMBA]](./Images/AMBA.jpg)

## Cortex-M Processor Profile

* Cortex-M0: Focused on minimal size and power consumption, ideal for ultra-low-power applications. (13 μW/MHz)
* Cortex-M0+: Even lower power than M0 with a shorter pipeline for faster wake-up times. (11 μW/MHz)
* Cortex-M3: Offers a good balance between performance and power, with a rich instruction set including Thumb-2 for efficient code density. (32 μW/MHz)
* Cortex-M4: Adds muscle for DSP (Digital Signal Processing) tasks and the option for a floating-point unit for more complex math.
* Cortex-M7: Prioritizes high performance for demanding embedded applications.
* Cortex-M23/M33: Integrate Arm TrustZone technology for enhanced security in security-critical applications.

## ARM Cortex-M4

![[CortexM4]](./Images/CortexM4.jpg)

![[CortexM4Block]](./Images/cortexM4Block.jpg)

### Processor Core Features:

* The Cortex-M4 core supports a subset of instructions from the Thumb instruction set, which is a compressed version of the ARM instruction set. This allows for more efficient code execution and reduced memory usage.
* The Cortex-M4 core has multiple stack pointers, each associated with different operating modes such as Handler mode and Thread mode. This allows the processor to efficiently switch between different contexts without having to manually manage the stack.
* The Cortex-M4 core includes hardware instructions for both signed (SDIV) and unsigned (UDIV) integer division operations. These instructions are implemented in hardware, providing faster execution compared to software-based division algorithms.
* The Cortex-M4 core supports different operating modes, including Handler mode for handling exceptions and interrupts, and Thread mode for executing regular application code. These modes provide different levels of privilege and access to system resources.
* The Cortex-M4 core supports both Thumb state, which uses 16-bit instructions for compact code, and Debug state, which allows debugging features such as breakpoints and watchpoints to be used during program execution.
* Certain instructions like LDM (Load Multiple), STM (Store Multiple), PUSH, and POP can be interrupted and resumed without loss of data or corruption. This feature helps in achieving low interrupt latency, which is crucial for real-time embedded systems.
* When an interrupt occurs, the Cortex-M4 core automatically saves the processor state (registers, program counter, etc.) before jumping to the Interrupt Service Routine (ISR). After the ISR completes, the core restores the saved state, allowing the interrupted code to resume execution seamlessly.
* The Cortex-M4 core can be configured to support either big-endian or little-endian memory accesses, depending on the ARMv6 variant used. This flexibility allows the core to interface with different types of memory systems or peripherals.

### Floating Point Unit:

1. **32-bit instructions for single-precision data-processing operations:** The FPU supports 32-bit instructions specifically designed for single-precision floating-point operations, which are commonly used with C float data types.
2. **Combined Multiply and Accumulate (Fused MAC) instructions:** This feature allows for increased precision in calculations by performing both multiplication and addition in a single instruction. It's particularly useful for signal processing and other applications requiring high accuracy.
3. **Hardware support for various floating-point operations:** The FPU provides hardware acceleration for essential floating-point operations including conversion between integer and floating-point formats, addition, subtraction, multiplication (with optional accumulation), division, and square root calculation.
4. **IEEE rounding modes:** The FPU supports IEEE standard rounding modes, such as rounding towards zero, rounding towards positive infinity, rounding towards negative infinity, and rounding towards nearest value (ties to even or odd).
5. **Dedicated single-precision registers:** The FPU includes 32 dedicated 32-bit single-precision registers for storing floating-point data. Additionally, these registers can be accessed as 16 double-word (64-bit) registers for operations requiring extended precision or handling larger values. This flexibility enables efficient handling of floating-point data in various applications.

### NVIC (Nested Vector Interrupt Controller):

1. **Low latency interrupt processing:** The NVIC is designed to minimize interrupt latency, ensuring that interrupts are handled quickly and efficiently without significant delays.
2. **External interrupts, configurable from 1 to 240:** The NVIC supports a configurable number of external interrupts, ranging from 1 to 240, allowing flexibility in system design to accommodate various interrupt sources.
3. **Configurable priority levels:** Interrupt priorities are configurable with varying numbers of priority bits, typically ranging from 3 to 8 bits. This flexibility enables developers to prioritize interrupts based on their importance and criticality to the system.
4. **Dynamic reprioritization of interrupts:** The NVIC allows for dynamic reprioritization of interrupts, enabling the system to adapt to changing conditions and prioritize critical events as needed.
5. **Priority grouping:** The NVIC supports priority grouping, which enables developers to define preempting and non-preempting interrupt levels. This feature allows for fine-grained control over interrupt handling, ensuring that higher priority interrupts can preempt lower priority ones when necessary.
6. **Automatic processor state saving and restoration:** When an interrupt occurs, the NVIC automatically saves the processor state upon entry to the interrupt service routine (ISR) and restores it upon exit. This process occurs with no additional instruction overhead, ensuring efficient interrupt handling without impacting performance.
7. **Optional Wake-up Interrupt Controller (WIC):** Some Cortex-M4 implementations may include a Wake-up Interrupt Controller (WIC), which provides support for ultra-low-power sleep modes. The WIC allows the processor to wake up from sleep mode in response to specific wake-up events, minimizing power consumption in battery-powered devices.


![[ProgrammersModel]](./Images/programmersModel.jpg)

>> <https://www.st.com/resource/en/datasheet/stm32f411re.pdf> Page no -16

![[memoryAndBus]](./Images/memoryAndBus.jpg)
