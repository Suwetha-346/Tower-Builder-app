# Tower Builder Game

## Overview
Tower Builder is a turn-based strategy game where players place weighted blocks on either side of a balance beam. The goal is to keep the tower stable. If the weight difference between the left and right sides exceeds a specified limit, the tower collapses and the player who placed the last block loses.

This application is implemented in Python and visualized using diagram-style graphics generated with Matplotlib.

---

## Features

- Two gameplay modes:
  - Player vs Computer
  - Player vs Player
- Random block weights (1–10)
- Real-time visual tower diagram after each move
- Stability check based on weight difference
- Automatic collapse detection
- Clean graphical representation of balance beam and blocks

---

## How the Game Works

1. The tower starts empty.
2. Each turn, a block with a random weight is generated.
3. The player chooses to place it on the left or right side.
4. The system calculates total weights on both sides.
5. If the weight difference exceeds the allowed limit, the tower collapses.
6. The player who caused the collapse loses.

---

## Stability Rule

The tower remains stable when:

| Left Total − Right Total | ≤ Maximum Allowed Difference

If:

| Left Total − Right Total | > Maximum Allowed Difference

The tower collapses.

---

## Technologies Used

- Python 3
- Matplotlib (for diagram visualization)
- Random module (for block generation)

---

## Requirements

Install required library:

```bash
pip install matplotlib
