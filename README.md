# blackjack-compiler-construction
A Blackjack card game implemented as part of the Compiler Construction course, demonstrating concepts like lexical analysis, parsing, syntax tree generation, and semantic actions.
# 🃏 Blackjack Card Game – Compiler Construction Project

This repository contains the implementation of a **Blackjack card game** developed during the **Compiler Construction** course.  
The project focuses on applying compiler design principles such as **lexical analysis**, **parsing**, and **syntax-directed translation** while building an interactive card game.

---

## 🎮 Project Overview

**Blackjack** is a popular casino card game where players compete against the dealer to get a hand value closest to **21** without exceeding it.

This project goes beyond simple game mechanics — it integrates **compiler construction concepts** to process commands, validate inputs, and control game flow using **parsing techniques**.

---

## 🛠️ Features

✅ Interactive command-line Blackjack game  
✅ Uses **lexical analysis** to tokenize user commands  
✅ Implements a **parser** to validate game actions  
✅ Semantic actions handle player moves and game rules  
✅ Dealer AI for automated responses  
✅ Built with **modular design** for readability and maintainability  

---

## 🧩 Key Compiler Construction Concepts Used

This project demonstrates how compiler techniques can be applied to game development:

### **1. Lexical Analysis (Scanner)**
- Tokenizes player commands like:

### **2. Syntax Analysis (Parser)**
- Uses context-free grammar rules to validate commands  
- Ensures players input **valid moves** only

### **3. Semantic Actions**
- Associates meaning with parsed commands  
- Implements Blackjack rules, e.g.:
- Calculate hand totals  
- Handle Aces as 1 or 11  
- Detect Blackjack & Bust conditions

### **4. Error Handling**
- Catches invalid inputs  
- Displays **friendly error messages** instead of crashing

---

## 📂 Repository Structure

```bash
blackjack-compiler-construction/
│── src/
│   ├── lexer.l            # Lexical analyzer
│   ├── parser.y           # Grammar & parsing rules (YACC/Bison)
│   ├── blackjack.c        # Core game logic
│   ├── deck.c             # Card deck management
│   └── utils.c            # Helper functions
│
│── include/
│   ├── blackjack.h        # Game header file
│   ├── tokens.h           # Token definitions
│   └── utils.h
│
│── docs/
│   ├── project-report.pdf # Project explanation & theory
│   └── grammar.txt        # Grammar rules used for parsing
│
│── test/
│   ├── input.txt          # Sample test commands
│   ├── output.txt         # Expected results
│
└── README.md
