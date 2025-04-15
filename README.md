# Vulnerable C Demo: Custom Stack Canary

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
