# Multiplayer Quiz Buzzer System

🏆 **Runner-Up, Junior Group — EEE Project Show Spring 2025, United International University**

A 4-player quiz buzzer system, built twice: first with pure digital logic (44 ICs, no microcontroller), then redesigned on an STM32 microcontroller.

## Round 1: Digital Electronics (Spring 2025)

Built with **44 logic ICs and no microcontroller**, hand-wired on breadboards and simulated in Proteus.

### Features

- First-press detection with lockout of the other players
- Winner's number shown on a 7-segment display, with LED and buzzer indication
- Reaction timer that pauses when a player presses
- 10-second answer timer; the display turns off automatically if time runs out
- Live scoreboard (0-8) per player with up/down counters
- Host controls: reset, correct/wrong marking, set by host

📄 Schematic: [docs/round1-schematic-44-ic.pdf](docs/round1-schematic-44-ic.pdf)

## Round 2: Microprocessor course (STM32F103C8T6)

The same idea rebuilt on an **STM32F103C8T6** with a 16x2 LCD, push buttons, LEDs and a buzzer. The logic that took 44 ICs moved into firmware, shrinking the hardware into one small module.

📄 Paper: [docs/round2-stm32-paper.pdf](docs/round2-stm32-paper.pdf) — *Design and Implementation of a Microcontroller Based Four-Player Quiz Buzzer System*

## What we learned

Hardware logic showed us exactly what happens inside the system. The microcontroller showed how much of that could be simplified with software.

## Team

Dipu Chandra Sarker, Md. Mazharul Islam Chowdhury, Zihadul Islam Shihab, Omar Faysal Ornob, Taslima Aktar

## Repository structure

```
docs/   schematic (Round 1) and paper (Round 2)
```
