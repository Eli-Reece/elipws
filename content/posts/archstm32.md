+++
date = '2024-03-22T17:20:53-08:00'
title = 'STM32 Arch Workflow'
toc = true
tocBorder = true
+++
## Hardware
- STM32 board
- ST-Link V2
## Install the tools
- CubeMX
- GNU ARM Embedded Toolchain
	- arm-none-eabi-gcc
	- arm-none-eabi-gdb
	- arm-none-eabi-newlib
- make
- OpenOCD
	- On-Chip Debugger software that will upload compiled code to the STM32
- vscode
	- stm32-for-vscode extension
## CubeMX Configuration

- Configure Project output to Makefile
```bash
Project Manager->Project->Toolchain/IDE
set to Makefile
```
- Set project to copy all used libraries to the project folder
```bash
Code Generator tab
enable 'Copy all use libraries into the project folder'
```
- Do whatever ever configuration then build
```bash
click 'GENERATE CODE'
```
## VSCode
- Open the project in vscode
- Write code
```bash
Use Extension Icon or Open the command palette (Ctrl+Shift+P) or Ctrl+Shift+B
Build STM32 Project
Flash STM32
```
# References
- https://gist.github.com/Bonnee/393c4be25d2e8620d9ec406073940d3a
