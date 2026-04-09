
# Interactive Turing Machine Simulator

This project is a web-based simulator that demonstrates how a Turing Machine processes input strings step by step. It is designed to visualize computation in a clear and interactive way, making theoretical concepts easier to understand.

The simulator works as a general-purpose engine. It does not rely on hardcoded examples. Every computation is driven entirely by the transition function provided by the user or predefined configurations.

## Features

- Step-by-step execution of the Turing Machine
- Automatic execution with controllable speed
- Visual representation of the tape and head movement
- Display of current state, symbol, and applied transition
- Support for both predefined and user-defined machines
- Dynamic tape expansion during execution
- Accept and reject state detection
- Transition history tracking

## How It Works

The simulator follows the formal definition of a Turing Machine. At each step, it reads the current symbol, finds the corresponding transition, updates the tape, moves the head, and changes the state. The process continues until it reaches an accept state, reject state, or no valid transition exists.

All machines, including predefined ones, use the same execution logic. This ensures that the simulator behaves consistently for any valid input.

## Predefined Machines

The application includes a set of ready-to-use machines to demonstrate common problems:

- Binary increment operation
- Palindrome checking
- Equal number of 0s and 1s

These machines are implemented using transition tables and are executed through the same engine as custom machines.

## Custom Turing Machine

Users can define their own machines by providing transitions in the required format:

{"state,symbol": ["newState","writeSymbol","direction"]}

The simulator processes these transitions dynamically and applies them to any valid input string.

## Usage

1. Enter an input string on the tape
2. Select a predefined machine or provide custom transitions
3. Click step to execute one transition at a time or run for continuous execution
4. Observe the tape updates, head movement, and state changes
5. The simulation stops when it reaches an accept or reject state

## Technologies Used

- HTML for structure
- CSS for layout and styling
- JavaScript for simulation logic and interactivity

## Deployment

The project can be deployed as a static site using platforms such as Vercel or Render. No build process is required.

## Purpose

This simulator is built to provide a practical understanding of computation models in Theory of Computation. It focuses on clarity, correctness, and dynamic behavior rather than fixed examples.
