# Operating System Project - Phase 2

This project is part of an academic course on operating systems, where we simulate an operating system's job scheduling and memory management functionalities. The project is implemented in C++ and includes key concepts such as paging, job scheduling, and error handling.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Error Handling](#error-handling)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This project simulates a simple operating system that can read job instructions, execute them, and manage memory using paging. It includes functionalities for reading input from files, processing instructions, handling errors, and logging the results.

## Features
- Job scheduling
- Memory management with paging
- Instruction execution (GD, PD, CR, SR, LR, BT)
- Error handling (Out of Data, Line Limit exceeded, Time Limit exceeded, Opcode Error, Operand Error, Invalid Page Fault)
- Logging and output generation

## Tech Stack
- **Programming Language:** C++
- **Libraries:** Standard C++ Libraries (iostream, fstream, string, vector, set)

## Prerequisites
- C++ compiler (g++ recommended)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/OmkarLolage21/OS_Phase2.git
   cd OS_Phase2
   ```

2. Ensure you have a C++ compiler installed. For g++:
   ```bash
   sudo apt-get install g++
   ```

## Usage
1. Compile the program:
   ```bash
   g++ main.cpp -o os_project
   ```

2. Create an input file `ip.txt` with job instructions in the project directory.

3. Run the executable:
   ```bash
   ./os_project
   ```

4. Output will be generated in the `output.txt` file.

## Error Handling
The program handles various errors and logs them appropriately:
- **Out of Data:** Occurs when the program tries to read beyond the available input data.
- **Line Limit Exceeded:** Occurs when the number of printed lines exceeds the defined line limit.
- **Time Limit Exceeded:** Occurs when the time taken to execute instructions exceeds the defined time limit.
- **Opcode Error:** Occurs when an invalid opcode is encountered.
- **Operand Error:** Occurs when an invalid operand is encountered.
- **Invalid Page Fault:** Occurs when an invalid page fault is encountered.

The error handling and logging are implemented in the `endExecution` function.

## Contributing
Contributions are welcome! Please follow these steps to contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
