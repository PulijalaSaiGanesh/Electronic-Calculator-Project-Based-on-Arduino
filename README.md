# Electronic Calculator Using Arduino

## Overview

This project implements a **Programmable Electronic Calculator** using an **Arduino Uno**, **4×4 Matrix Keypad**, and **16×2 LCD Display**. The calculator is capable of performing both **arithmetic** and **trigonometric operations** through a user-friendly keypad interface.

When a user enters numbers through the keypad, the input is displayed on the LCD screen. Different mathematical operations can be selected using dedicated keypad buttons, and the calculated result is displayed instantly on the LCD.

The project demonstrates the practical implementation of embedded systems concepts such as keypad interfacing, LCD interfacing, user input processing, mathematical computations, and real-time display management using Arduino.

---

## Features

### Arithmetic Operations

* Addition (+)
* Subtraction (-)
* Multiplication (×)
* Division (÷)
* Power (xʸ)
* Square (x²)

### Trigonometric Operations

* Sine (sin)
* Cosine (cos)
* Tangent (tan)

### Additional Functionalities

* Supports positive and negative numbers
* Decimal number input
* Automatic scrolling for long expressions
* Error handling for invalid operations (e.g., division by zero)
* Optimized result formatting with floating-point precision control
* Startup loading animation on LCD

---

## Hardware Components Required

* Arduino Uno
* 4×4 Matrix Keypad
* 16×2 LCD Display (HD44780 Compatible)
* Jumper Wires
* Breadboard
* USB Cable for Arduino Programming

---

## Keypad Layout

```text
1  2  3  A
4  5  6  B
7  8  9  C
*  0  #  D
```

---

## Key Functions

| Key | Function                        |
| --- | ------------------------------- |
| A   | Select Next Operation           |
| B   | Select Previous Operation       |
| C   | Clear Calculator                |
| D   | Enter / Execute Operation       |
| *   | Decimal Point (.)               |
| #   | Toggle Positive/Negative Number |

### Available Operations

| Operation Code | Function       |
| -------------- | -------------- |
| +              | Addition       |
| -              | Subtraction    |
| ×              | Multiplication |
| ÷              | Division       |
| ^              | Power          |
| ^2             | Square         |
| sin            | Sine           |
| cos            | Cosine         |
| tan            | Tangent        |

---

## Circuit Connections

### Keypad Connections

| Keypad Pin | Arduino Pin |
| ---------- | ----------- |
| Row 0      | D2          |
| Row 1      | D3          |
| Row 2      | A4          |
| Row 3      | A5          |
| Column 0   | D4          |
| Column 1   | D5          |
| Column 2   | D6          |
| Column 3   | D7          |

### LCD Connections

| LCD Pin | Arduino Pin |
| ------- | ----------- |
| RS      | D13         |
| EN      | D12         |
| D4      | D11         |
| D5      | D10         |
| D6      | D9          |
| D7      | D8          |
| VCC     | 5V          |
| GND     | GND         |

For complete wiring details, refer to the `calculator_pins.txt` file.

---

## Software Requirements

* Arduino IDE **or**
* Visual Studio Code with PlatformIO Extension

### Required Libraries

```cpp
Keypad.h
LiquidCrystal.h
stdlib.h
math.h
```

---

## Project Structure

```text
├── CompleteCode.txt        # Main Arduino calculator source code
├── calculator_pins.txt     # Hardware wiring and pin configuration
├── README.md               # Project documentation
```

---

## How to Run

1. Clone this repository.
2. Open the project using **Arduino IDE** or **VS Code with PlatformIO**.
3. Connect the Arduino Uno to your computer.
4. Verify the pin connections according to `calculator_pins.txt`.
5. Build/Compile the project.
6. Upload the code to the Arduino board.
7. Power the circuit and start performing calculations.

---

## Note

* Some editors may show syntax warnings when opening the source file. These can usually be ignored if the project builds successfully.
* Always use the **Build/Verify** option before uploading the code to confirm there are no compilation errors.
* Trigonometric calculations are performed in degrees.
* The LCD operates in an 8×2 display mode with scrolling support for longer expressions.

---

## Learning Outcomes

This project helps in understanding:

* Arduino Programming
* Embedded Systems Design
* LCD Interfacing
* Matrix Keypad Interfacing
* Mathematical Function Implementation
* User Interface Design for Embedded Systems
* Real-Time Input Processing

---

## Future Enhancements

* Scientific calculator mode
* Memory storage functions
* More advanced mathematical operations
* OLED/TFT display support
* Battery-powered portable version
* Menu-driven user interface

---

## Author

Developed as an Embedded Systems Project using Arduino to demonstrate practical implementation of a programmable calculator with arithmetic and trigonometric capabilities.

