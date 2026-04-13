# 🃏 Blackjack Game (Python - Capstone Project)

A command-line Blackjack game built using Python, where the player competes against a computer dealer using standard Blackjack rules.

This project demonstrates core Python concepts like functions, loops, conditionals, and randomization in a fun and interactive way.

---

## 🎮 Game Overview

This is a terminal-based Blackjack game where:

- You are the player 🧑
- The computer acts as the dealer 🤖
- The goal is to get as close to 21 as possible without going over

---

## 🧠 Game Logic (How it Works)

### 🔹 Card Dealing
- Cards are randomly selected using Python's `random` module
- Both player and computer receive **2 cards initially**

### 🔹 Score Calculation
- Aces (11) automatically convert to 1 if total exceeds 21
- A Blackjack (Ace + 10) is represented as **0 score**

### 🔹 Player Turn
- Choose:
  - `'y'` → draw another card (Hit)
  - `'n'` → stop (Stand)

### 🔹 Dealer (Computer) Logic
- The dealer keeps drawing cards until:
  - Score is **at least 17**
  - Or gets Blackjack

### 🔹 Winning Conditions
- Closest to 21 wins
- Going over 21 → automatic loss
- Blackjack beats normal score

---

## 🏠 House Rules

- Infinite deck (cards are not removed after drawing)
- No jokers
- Face cards (J, Q, K) = 10
- Ace = 11 or 1 (auto-adjusted)
- Equal probability for all cards

```python
cards = [11, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10]
