# ssdtmeme
### note: i have personally used a modified version of this project on valorant for over 8+ months. it is indeed effective
ssdtmeme is a kernel-mode driver designed to hook the System Service Dispatch Table (SSDT) in Windows. The driver is divided into several files that each represent a separate code block, including the driver entry point, the SSDT hooking function, and the communication methods.

## Driver Entry Point

The driver entry point is the starting point of the driver code. It initializes the driver and registers the driver with the Windows operating system. The entry point also creates the communication method that will be used to communicate between usermode and kernelmode. The communication method is designed to be undetected by anti-cheat software, allowing the driver to bypass BattlEye and EasyAntiCheat.

## SSDT Hooking Function

The SSDT hooking function is the core of the driver. It is responsible for hooking the SSDT and redirecting calls to specific system services to custom implementation. The hooking function replaces the original SSDT entry with a pointer to the custom implementation. This allows the driver to intercept and modify system calls made by other programs, such as game cheat engines. 

## Communication Methods

The communication methods are used to enable communication between usermode and kernelmode. The driver was (in the past tense) an undetected communication method to bypass BattlEye and EasyAntiCheat. This allows the driver to communicate with usermode without being detected by anti-cheat software.

