# Mirai Botnet

This repository offers an **educational implementation** of the infamous Mirai botnet, originally discovered in 2016. Mirai targeted IoT (Internet of Things) devices like cameras and routers, turning them into a large botnet used for massive Distributed Denial-of-Service (DDoS) attacks. This project demonstrates vulnerabilities in IoT devices and stresses the critical need for **network security** and **secure coding practices**.

## History
Mirai was initially developed by Paras Jha, who released the source code in 2016 after using it to launch one of the largest DDoS attacks in history. It exploited weak, default credentials in IoT devices, which allowed attackers to control thousands of devices remotely. The botnet's ability to spread rapidly across unsecured networks led to devastating effects, influencing how the industry approached IoT security.

## Features
- **Command and Control (C&C):** A lightweight C&C server to simulate botnet operations.
- **Exploitation of Weak Credentials:** The botnet scans and infects IoT devices with weak or default passwords.
- **Cross-Architecture Support:** Support for multiple architectures like ARM, MIPS, etc.
- **Network Stress Testing:** Highlighting how DDoS attacks can overload systems and affect network infrastructure.

## Requirements
- Python 3.x
- GCC compiler
- Linux environment (tested on Ubuntu/Debian)
- Cross-compilation toolchains (for different architectures like ARM, MIPS)
- Knowledge of IoT security

## Installation Guide

1. **Set up your environment:**
   - Ensure you have a **Linux** system (tested on Ubuntu/Debian).
   - Install Python 3.x and the GCC compiler:
     ```bash
     sudo apt update
     sudo apt install python3 gcc
     ```
   - Install cross-compilation toolchains (for ARM, MIPS, etc.):
     ```bash
     sudo apt install gcc-arm-linux-gnueabi gcc-mips-linux-gnu
     ```

2. **Download and compile the source:**
   - Clone this repo:
     ```bash
     git clone https://github.com/yourrepo/mirai-botnet
     cd mirai-botnet
     ```
   - Compile the code for different architectures:
     ```bash
     make
     ```

3. **Run the Command & Control server:**
   - Launch the server and start assigning commands to infected devices.

4. **Simulate Botnet Attacks:**
   - Use the included scripts to simulate a basic DDoS attack. **Note**: Always do this in a controlled, safe environment.

## Usage
The botnet works by scanning IP addresses for devices with open telnet ports. Once it identifies vulnerable devices (using weak default credentials), it will attempt to gain access and install the bot payload.  
You'll need to launch the C&C server, configure the bot to report back to the server, and start testing **on systems you own or have permission to experiment with**.

## Risks & Security Warnings
- **Unauthorized Testing:** Never run the botnet on any public networks or without explicit permission.
- **Legal Consequences:** Engaging in unauthorized testing may violate laws and lead to serious legal action.

## Conclusion
This project serves as a **learning tool** for understanding how botnets like Mirai function and highlights the importance of **strengthening IoT security**. It should only be used in an **ethical, controlled environment** for research purposes.

## Disclaimer
This project is **for educational purposes only**. Do not use this on any system or network you do not own or have explicit permission to test. Unauthorized use of this code may violate cybersecurity laws and lead to severe legal consequences. The authors are not responsible for any misuse or damage caused.
