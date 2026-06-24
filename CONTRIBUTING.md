# Contributing to COA Lab Programs

Thank you for your interest in contributing to this repository! This is an educational collection of x86-64 NASM Assembly and SAS Simulator programs for the Computer Organization and Architecture (COA) lab.

---

## How to Contribute

### Types of Contributions Welcome

- **New lab programs** — Additional assembly programs (NASM or SAS) covering COA topics
- **Bug fixes** — Corrections to existing assembly code
- **Documentation improvements** — Better comments, README enhancements
- **Makefile** — Automated build scripts for NASM programs
- **Sample I/O** — Adding expected input/output examples for each program

---

## Getting Started

### 1. Fork the Repository

Click the **Fork** button on the top right of this repository page.

### 2. Clone Your Fork

```bash
git clone https://github.com/YOUR_USERNAME/COA.git
cd COA
```

### 3. Create a Feature Branch

```bash
git checkout -b feature/add-sorting-program
```

Use descriptive branch names:
- `feature/add-bubble-sort-nasm`
- `fix/hex-to-bcd-overflow`
- `docs/improve-readme`

---

## Submitting a New Assembly Program

### NASM Program Checklist

Before submitting a new `.asm` file, ensure:

- [ ] File includes a **header comment** describing the program purpose
- [ ] Code is **well-commented** at each logical section
- [ ] Program compiles with: `nasm -f elf64 filename.asm -o filename.o`
- [ ] Program links with: `ld -o filename filename.o`
- [ ] Program runs correctly on Linux x86-64
- [ ] README.md Programs Overview table is updated

### SAS Program Checklist

Before submitting a new `.sas` file, ensure:

- [ ] File includes a **header comment** with program description
- [ ] Program runs correctly in the SAS simulator
- [ ] README.md is updated accordingly

### Naming Conventions

Follow the existing naming pattern:

| Type | Format | Example |
|------|--------|---------|
| NASM files | `<number>_<abbreviation>.asm` | `12_BS.asm` (Bubble Sort) |
| SAS files | `<OPERATION>.sas` | `DIV.sas` |

---

## Commit Message Guidelines

Use clear and descriptive commit messages:

```
feat: Add bubble sort implementation in x86-64 NASM
fix: Correct BCD overflow in hex-to-bcd conversion
docs: Update README with 8086 program descriptions
refactor: Simplify string reverse loop in 11_SRSP.asm
```

Format: `<type>: <short description>`

Types:
- `feat` — New feature or program
- `fix` — Bug fix
- `docs` — Documentation only
- `refactor` — Code restructuring without behavior change
- `test` — Adding test cases or sample I/O

---

## Pull Request Process

1. Ensure your code follows the checklist above
2. Update the README.md if you added a new program
3. Create a pull request with a clear title and description
4. Reference any related issues: `Closes #12`
5. Wait for review

---

## Code Style

### NASM Assembly

- Use **lowercase** for instructions (`mov`, `add`, `cmp`)
- Use **meaningful label names** (`convert_loop`, `print_result`)
- Add section headers as comments:
  ```asm
  ;; ---- Input Section ----
  ;; ---- Processing ----
  ;; ---- Output Section ----
  ```
- Always include a program header comment:
  ```asm
  ;; Program: Bubble Sort in x86-64 NASM Assembly
  ;; Description: Sorts an array of 10 integers using bubble sort
  ;; Author: Your Name
  ```

---

## Questions?

Open an [issue](https://github.com/tusharkkp/COA/issues) with the label `question` and the maintainer will respond.

---

*Happy coding! Low-level programming builds strong foundations.*
