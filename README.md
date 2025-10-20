# Dictionary Worder

### Description

I wanted a simple program that I could run easily that would broaden my vocabulary, so I made this as both an exercise and a tool.

The app takes words from dictionary/dictionary.csv and spits them out along with their definitions
You're able to set how many words you want the program to return from the settings/settings.csv file

It'll output the words in this format:

```
> > Word #0 is [word].  Getting definitions:
> > > > Definition #1: [definition].
```

## How to Run

**Prerequisites:** C++17 or later compiler

**Build:**

```bash
g++ main.cpp -std=c++17
```

**Run:**

```bash
./a.out
```

On first run, the program will ask how many words you want to see per session. This preference is saved automatically.

## Dictionary CSV Format

The program expects `dictionary/dictionary.csv` with this structure:

```
word,part_of_speech,definition
```

**Example:**

```
computer,noun,the thing you are using to read this repository
ephemeral,adjective,lasting for a very short time
```

**Note:** The part of speech field (column 2) is required but not currently displayed.

## What I Learned

- File I/O and CSV parsing in C++
- Using `std::filesystem` for cross-platform file handling
- Proper random number generation with Mersenne Twister
- Input validation with try-catch blocks
- Building modular file utilities with custom headers
