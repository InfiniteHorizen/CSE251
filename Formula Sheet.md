---
title: "Formula Sheet"
date: 2026-10-04
course: CSE 251
tags: [cse251, formulas, reference]
aliases: [Formulas, Cheat Sheet]
---

# Formula Sheet

Running list, updated after each lecture. Each entry says where it came from.

## Potential and ground

Potential difference across any two-terminal element:

$$V = V_{(+)} - V_{(-)}$$

Ground ($0\ \text{V}$) can be any point. Choosing a different one shifts node voltages but not voltage differences, currents or power.

*From:* [Lecture 01](Lectures/2026-10-04%20Lecture%2001%20-%20Line%20Circuit%20Representation.md)

## Removing a source on a line circuit

| Situation | Action |
|---|---|
| − end of the source on ground | + end is at $+V$; delete source, label the point $+V$ |
| + end of the source on ground | − end is at $-V$; delete source, label the point $-V$ |
| Neither end on ground | Cannot delete; keep it drawn |

Never keep the ground wire after replacing a cell with a label (short circuit).

## Ohm's law and power (resistors only)

$$V = IR, \qquad P = \frac{V^2}{R} = I^2 R = VI$$

Ideal voltage source: $R = 0$. Ideal current source: $R = \infty$. Do not apply $V = IR$ or $P = I^2R$ to an ideal battery.

## Current on a line circuit

Single resistor between nodes $V_1$ and $V_2$:

$$I_{1 \to 2} = \frac{V_1 - V_2}{R}$$

Path with sources:

$$I = \frac{V_{start} - V_{end} - \sum V}{\sum R}$$

$\sum V$: count $+V$ for a source entered at its **+** terminal, $-V$ for one entered at its **−** terminal. Reversing the direction flips the sign of $I$.

## KVL sign convention on a line diagram

| Element | Term |
|---|---|
| Node you leave (start) | $-V_{start}$ |
| Node you enter (end) | $+V_{end}$ |
| Resistor | $+IR$ |
| Source entered at + | $+V$ |
| Source entered at − | $-V$ |

$$-V_1 + IR_1 + V_{battery} + IR_2 + V_2 = 0$$

Related: [Course Index](INDEX.md), [Lecture 01](Lectures/2026-10-04%20Lecture%2001%20-%20Line%20Circuit%20Representation.md)
