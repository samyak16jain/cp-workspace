# cp-workspace

## Overview

A minimal workspace for solving Codeforces problems in C++ locally and submitting on the Codeforces website.

## Prerequisites

### macOS

```bash
brew install gcc
```

### Ubuntu

```bash
sudo apt install g++
```

## Compile

```bash
g++ -std=c++23 -I. main.cpp -o main
```

On macOS, use Homebrew GCC (plain `g++` is Clang):

```bash
g++-15 -std=c++23 -I. main.cpp -o main
```

The `-I.` flag picks up the local `bits/stdc++.h` shim. Codeforces provides this header natively — only submit `main.cpp`, not the `bits/` folder.

## Run

```bash
./main < input.txt
```

## Workflow

1. Open a Codeforces problem.
2. Write the solution in `main.cpp`.
3. Copy sample input into `input.txt`.
4. Run locally.
5. Submit `main.cpp` on Codeforces.
6. Repeat for the next problem.

## Philosophy

* Keep the workspace simple.
* Focus on solving problems.
* Add tooling only when it becomes necessary.
