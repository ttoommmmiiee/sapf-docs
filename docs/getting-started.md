---
sidebar_position: 2
---

# Getting Started

### Installation
1. Place the sapf binary in ~/bin or preferred location
2. Remove Apple's quarantine attribute:
```bash
xattr -r -d com.apple.quarantine <path-to-sapf-binary>
```

### Environment Setup
Add to your shell profile:
```bash
export SAPF_HISTORY="$HOME/sapf-files/sapf-history.txt"
export SAPF_LOG="$HOME/sapf-files/sapf-log.txt" 
export SAPF_PRELUDE="$HOME/sapf-files/sapf-prelude.txt"
export SAPF_EXAMPLES="$HOME/sapf-files/sapf-examples.txt"
export SAPF_README="$HOME/sapf-files/README.txt"
export SAPF_RECORDINGS="$HOME/sapf-files/recordings"
export SAPF_SPECTROGRAMS="$HOME/sapf-files/spectrograms"
```

### Command Line Usage
```bash
sapf [-r sample-rate] [-p prelude-file]
sapf [-h]
```

Options:
- `-r sample-rate`: Sets session sample rate (default: 96000 Hz)
- `-p prelude-file`: Path to initialization code
- `-h`: Print help

## Language Basics

### Basic Syntax
SAPF uses postfix notation where operators follow their operands:
```
2 3 *  -->  6
```

### Comments
```
; Single line comment
```

### Numbers
```
# Basic numbers
1  2.3  .5  7.

# Scientific notation
3.4e-3  1.7e4

# Suffixes
2pi      # Multiply by π
1M       # Mega (×1000000)
4k       # Kilo (×1000)
8h       # Hecto (×100)
386c     # Centi (×0.01)
53m      # Milli (×0.001)
20u      # Micro (×0.000001)

# Fractions
5/4  9/7  15/11  pi/4
```

[Continued in next message due to length...]