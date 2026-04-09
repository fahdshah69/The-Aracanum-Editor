# The Arcanum Editor 🖋️

The Arcanum Editor is a custom built desktop text editor developed using C++ and the Win32 API. It is designed from the ground up to handle text manipulation, dynamic layout configuration, and real-time document parsing without relying on standard GUI text-box controls.

## 🚀 Features

* **Dynamic Text Reflow:** Automatically adjusts and wraps text based on configured layout parameters (max columns, max lines per column, and max characters per line).
* **Real-time Statistics:** Includes built-in word and sentence counting capabilities.
* **Search Functionality:** Quickly locate specific strings of text within the document structure.
* **Custom Layout Configuration:** Granular control over the page grid and text boundaries.

## Architecture & Constraints

This project was built adhering to strict Object-Oriented Programming (OOP) principles and specific architectural constraints to ensure encapsulated and modular code:

* **Strict OOP:** Zero global functions are used throughout the entire codebase.
* **No Inline Keyword:** The `inline` keyword is strictly avoided to enforce proper translation unit compilation.
* **Consolidated Codebase:** The entire application logic is contained within a single header file (`submission.h`) and executed via `main.cpp`.

### Data Structure Hierarchy
The text grid is managed through a deeply nested, custom class hierarchy rather than simple string arrays:
`Editor` ➔ `Document` ➔ `Page` ➔ `Column` ➔ `Line`

## 🛠️ Getting Started

### Prerequisites
* A Windows operating system.
* A C++ compiler that supports the Win32 API (e.g., MSVC via Visual Studio, or MinGW).

### Building the Project
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/arcanum-editor.git](https://github.com/yourusername/arcanum-editor.git)
