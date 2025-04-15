# Vulnerable C Demo: Custom Stack Canary

## Future Work

1. **Explore Other Vulnerability Types and Mitigation Techniques**
   - **Integer Overflows/Underflows:** Demonstrating potential pitfalls with arithmetic operations.
   - **Format String Vulnerabilities:** Examples and safe coding practices.
   - **Use-After-Free/Double Free:** Understanding dynamic memory management pitfalls.
   - **Race Conditions:** Investigating concurrency issues in C programming.
   
2. **Investigate Modern Memory Safety Mechanisms**
   - **Address Sanitizer (ASan):** Using ASan to detect and debug memory issues.
   - **Memory Safe Languages:** Exploring secure alternatives like Rust.
   - **Control Flow Integrity (CFI):** Researching compiler and hardware-level security features.
   - **Hardware-based Protections:** Examining features such as the NX bit and DEP.


## Overview
This project demonstrates a simple vulnerability in C programming—the buffer overflow—and shows how a custom stack canary can be used to detect an attack. It is designed for educational purposes.

## Disclaimer
**WARNING:** This code is intentionally insecure and is for educational use only. Do not use it in production or for any malicious activities.

## Features
- Demonstrates buffer overflow through an unsafe use of `strcpy()`.
- Implements a custom stack canary mechanism to detect overflow.
- Provides a hands-on example for understanding low-level C programming and vulnerability exploitation.

## Setup and Usage

### Prerequisites
- GCC compiler
- Visual Studio Code for editing, building, and debugging

### Compilation
To compile the program using GCC without the built-in stack protector:
```bash
gcc -fno-stack-protector -o stack_canary_demo stack_canary_demo.c


