# Friday-Turtle
Ghost PDF


## Phase 1: Environment & Toolchain Setup

First, we must prepare Termux with the necessary compilers and debugging tools.

```
# 1. Update and Upgrade the environment
pkg update && pkg upgrade -y

# 2. Install the Toolchain (Compilers, Debuggers, and Analysis tools)
pkg install python clang make binutils git -y

# 3. Install Python-specific libraries for the Orchestrator
pip install requests cryptography
```



## Phase 2: The Core Engine (The Exploit Logic)

We will create the three essential modules: the Trigger (to bypass security), the Bypass (to manage memory), and the Stealth (to handle the fileless nature).

## Step 1: Create the Exploit Module (engine.c)

This module handles the memory corruption and the ROP chain logic.

```
