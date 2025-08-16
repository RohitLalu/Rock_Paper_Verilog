# Rock_Paper_Verilog

Rock_Paper_Verilog is a digital implementation of the classic Rock-Paper-Scissors game using Verilog HDL. This repository contains the source code, testbenches, and simulation instructions to run the game logic on FPGA or in simulation environments.

## Overview

- **Language:** Verilog HDL
- **Purpose:** Demonstrates finite state machine (FSM) and basic digital logic design for a fun, interactive project.
- **Features:** 
  - User input selection (Rock, Paper, or Scissors)
  - Random computer choice generation
  - Outcome determination logic (Win, Lose, Draw)
  - Display or LED output (if applicable for your board)

## Getting Started

1. **Clone the repository**
    ```sh
    git clone https://github.com/RohitLalu/Rock_Paper_Verilog.git
    ```

2. **Explore the Source Code**
    - All Verilog modules are in the `src/` directory.
    - Testbenches (for simulation) can be found in the `test/` directory.

3. **Simulation**
    - Use any Verilog simulator (e.g., ModelSim, Icarus Verilog).
    - Example command:
      ```sh
      iverilog -o game_testbench src/game.v test/game_tb.v
      vvp game_testbench
      ```

4. **FPGA Synthesis**
    - The design can be synthesized for most FPGA boards. Pin mappings and constraints will need to be adjusted for your specific hardware.

## Directory Structure

```
Rock_Paper_Verilog/
├── src/         # Verilog source files
├── test/        # Testbench files
├── README.md
└── ...
```

## How It Works

1. The user selects Rock, Paper, or Scissors via input switches/buttons.
2. The computer generates a random selection.
3. The game logic compares choices and determines the result.
4. The outcome is displayed via LEDs or seven segment display.

## Contributing

Pull requests are welcome! If you have suggestions for improvements or new features, feel free to fork the repository and submit a PR.

## License

This project is licensed under the MIT License.

## Author

- [RohitLalu](https://github.com/RohitLalu)

---
Enjoy playing Rock-Paper-Scissors in hardware!
