# CodeAdvent

A small collection of Advent-style puzzle solutions written in C# as a single console application.

## Overview

This repository contains a simple console program (Program.cs) that constructs and runs seven puzzle solver classes:

- Advent
- Advent2
- Advent3
- Advent4
- Advent5
- Advent6
- Advent7

Each class reads an embedded test/input string, performs computations, and prints results to the console. Output lines are printed in the form:
- `del 1: <value>` — result for part 1 of that day's puzzle
- `del 2: <value>` — result for part 2 (when implemented)

Note: The input strings in Program.cs are inline and in some places truncated in the repository view. If you have full inputs, replace the truncated strings in Program.cs or modify the code to load external input files.

## Requirements

- .NET 6.0 SDK or later
- A C#-aware editor (Visual Studio, VS Code, Rider, etc.)

The project uses top-level statements and should build on modern .NET SDKs (6+).

## Build & Run

From the repository root (where `Program.cs` is located):

1. Restore and build:
   - dotnet build

2. Run the program:
   - dotnet run

You should see console output with multiple `del 1:` and `del 2:` lines — one pair for each Advent class (when the class prints both parts).

## Project Structure

- Program.cs — main entry point. Creates instances of each Advent class and prints their outputs.
- Advent, Advent2, ..., Advent7 — classes implementing different puzzle logic. They read inline string inputs in their constructors.

## Notes & Suggestions

- Inputs are currently embedded in code. For easier testing and maintenance, consider moving puzzle inputs into separate files (e.g., `inputs/day1.txt`) and update the code to read from them.
- Some test strings appear truncated in the repository view — verify the full inputs are present if you rely on those values.
- Consider splitting each day's solution into its own file and adding unit tests for correctness.
- Add null- and bounds-safety checks where appropriate (some code uses direct indexing) and prefer more descriptive naming (English names) if sharing this project.

## Contributing

Feel free to open issues or PRs to:
- Add missing inputs,
- Extract inputs to files,
- Add unit tests,
- Improve performance and readability.

---
