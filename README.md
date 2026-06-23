# UART Device Driver Development for STM32F411

## Overview

This repository contains the development of a UART device driver for the STM32F411 microcontroller using Embedded C and register level programming.

The project demonstrates the evolution of UART communication from basic polling techniques to interrupt driven communication and DMA based data transfer.

Each stage builds upon the previous implementation to provide a deeper understanding of UART communication, interrupt handling, DMA configuration, and peripheral driver development.

## Features

* UART Transmission using Polling
* UART Reception using Polling
* UART Reception using Interrupts
* UART Transmission using DMA
* DMA Transfer Complete Interrupt Handling
* NVIC Configuration
* USART Peripheral Configuration
* DMA Controller Configuration
* Memory Mapped I/O Programming

## Project Structure

```text
UART_Device_Driver_Development/
│
├── 01_UART_TX_Polling/
├── 02_UART_RX_Polling/
├── 03_UART_RX_Interrupt/
├── 04_UART_TX_DMA/
└── docs/
```

## Learning Progression

### Stage 1: UART TX Polling

Implemented UART transmission by monitoring the TXE flag and writing data to the USART data register.

### Stage 2: UART RX Polling

Implemented UART reception by monitoring the RXNE flag and reading data from the USART data register.

### Stage 3: UART RX Interrupt

Implemented interrupt driven UART reception using NVIC configuration and Interrupt Service Routines (ISR).

### Stage 4: UART TX DMA

Implemented DMA based UART transmission using DMA1 Stream6 Channel4 to transfer data from memory to the USART data register with minimal CPU intervention.

## Documentation

The `docs` directory contains detailed explanations for every stage of development, including:

* UART Transmission using Polling
* UART Reception using Polling
* UART Reception using Interrupts
* UART Transmission using DMA
* Register Configuration
* NVIC Configuration
* DMA Configuration
* Driver Architecture and Code Walkthroughs

## Concepts Demonstrated

* Embedded C Programming
* UART Communication
* Interrupt Handling
* DMA Transfers
* NVIC Configuration
* Memory Mapped I/O
* ARM Cortex M4 Fundamentals
* Peripheral Driver Development

## Target Microcontroller

STM32F411 Series Microcontroller
