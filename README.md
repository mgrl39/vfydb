<div align="center">

# 📚 VFYDB - Exercise Database for VFY

<img src="https://img.shields.io/badge/language-C-blue.svg" alt="Language C">
<img src="https://img.shields.io/badge/exercises-Structured-orange.svg" alt="Exercises">
<img src="https://img.shields.io/badge/levels-0--X-lightgrey.svg" alt="Levels">
<img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License MIT">

**A curated set of C programming exercises to be used with the [VFY](https://github.com/mgrl39/vfy) tool.**

</div>

---

## 🧭 Overview

This repository contains programming exercises organized by levels. It's designed to work seamlessly with the **[VFY](https://github.com/mgrl39/vfy)** tool, allowing learners to practice and verify their C coding skills.

Each exercise includes:

- `subject.txt` – A clear problem statement
- `expected_output.txt` – The correct output for verification
- `template.c` – A starter code template

---

## 📂 Structure

```
vfydb/
├── level_0/
│   ├── echo/
│   │   ├── subject.txt
│   │   ├── expected_output.txt
│   │   └── template.c
│   └── ...
├── level_1/
│   └── ...
└── level_n/
    └── ...
```

Each `level_X/` contains multiple exercises named after their goal or function (e.g., `vfy_strlen`, `echo`, `strcpy_rev`, etc.).

---

## ✍️ Creating a New Exercise

To contribute or add your own exercises, follow this format:

1. Create a folder under the appropriate level:
   ```
   level_1/my_exercise/
   ```

2. Inside, add the required files:
   - `subject.txt`  
     > Must include:
     - Title (`#`)
     - Description (`## Task`)
     - Examples (`## Examples` with shell-like usage)
   - `expected_output.txt`  
     > The exact output that your program should produce.
   - `template.c`  
     > Starter C code with headers and a basic structure.

---

## 🔗 Integration with VFY

To use this database with [VFY](https://github.com/mgrl39/vfy):

```bash
# In the vfy repo:
sudo make get-subjects
```

Or manually clone it:

```bash
git clone https://github.com/mgrl39/vfydb.git ~/.vfy/subjects
```

---

## 🌱 Example

An example from `level_0/echo/`:

**subject.txt**
```
# ECHO

## Task
Create a program that displays all its arguments, each followed by a newline.
Arguments should be displayed in the same order they are received.
If no arguments are provided, the program should display nothing.

## Examples
$ ./echo Hello World
Hello
World
$ ./echo "One" "Two" "Three"
One
Two
Three
$ ./echo
(displays nothing)
```

**expected_output.txt**
```
Hello
World
```

**template.c**
```c
#include <unistd.h>

int main(int argc, char *argv[])
{
    // Your code here

    return 0;
}
```

---

<div align="center">

**Happy Coding! Contribute new challenges and grow the VFY ecosystem.**  
🔗 [Back to VFY](https://github.com/mgrl39/vfy)

</div>
