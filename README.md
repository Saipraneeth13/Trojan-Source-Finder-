# Trojan Source Finder

## Overview

Trojan Source Finder is a cybersecurity-focused static analysis tool developed to detect Trojan Source vulnerabilities and hidden Unicode-based attacks within source code files and repositories.

Trojan Source attacks exploit Unicode bidirectional (BiDi) control characters to visually manipulate source code, making malicious code appear harmless to developers during code reviews while behaving differently during execution. These attacks can introduce hidden vulnerabilities, backdoors, or logic manipulation without obvious visual indicators.

This project aims to strengthen secure software development practices by automatically identifying suspicious Unicode patterns, hidden control characters, and deceptive code structures that could lead to Trojan Source attacks.

---

# What is a Trojan Source Attack?

A Trojan Source attack uses invisible or misleading Unicode bidirectional characters to alter how source code appears visually without changing how it is compiled or interpreted.

For example:

- A developer may see one logical flow of code.
- The compiler may interpret an entirely different flow.
- Hidden malicious instructions can bypass manual code reviews.

This type of attack can affect multiple programming languages and development environments.

---

# Key Features

- Detects Trojan Source vulnerabilities in source code
- Identifies hidden Unicode bidirectional characters
- Performs automated static code analysis
- Scans repositories recursively for malicious patterns
- Generates detailed vulnerability reports
- Supports secure code review workflows
- Detects visually deceptive source code structures
- Lightweight and fast security scanning tool

---

# Objectives

- Improve secure software development practices
- Detect hidden Unicode-based attacks automatically
- Reduce manual code review complexity
- Prevent malicious logic injection in source code
- Strengthen cybersecurity awareness in development workflows

---

# Supported Vulnerability Checks

The scanner detects:

- Bidirectional Unicode Override Characters
- Hidden Directional Formatting Characters
- Invisible Unicode Manipulation
- Suspicious Encoding Patterns
- Visual Code Reordering Attacks
- Potential Source Code Obfuscation

---

# Supported Programming Languages

The tool can scan source files written in:

- Python
- Java
- JavaScript
- C/C++
- Go
- Rust
- PHP
- HTML/CSS

Additional language support can be added easily.

---

# Tech Stack

## Programming Language
- Python

## Cybersecurity Concepts
- Static Code Analysis
- Secure Code Review
- Vulnerability Detection
- Unicode Security Analysis

## Libraries & Utilities
- Regex
- File System Traversal
- Encoding Analysis

---

# How Trojan Source Attacks Work

Trojan Source attacks exploit Unicode bidirectional text rendering rules.

Attackers insert hidden Unicode control characters such as:

```text id="fjlwmq"
U+202E  RIGHT-TO-LEFT OVERRIDE
U+202D  LEFT-TO-RIGHT OVERRIDE
U+2066  LEFT-TO-RIGHT ISOLATE
U+2067  RIGHT-TO-LEFT ISOLATE
