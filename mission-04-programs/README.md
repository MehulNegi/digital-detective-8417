# Mission 4 — How programs run

## 1. Task / objective

Create and run a simple Python program. Compare how a compiler and an interpreter handle program instructions.

## 2. Work completed

### Task 4.1 — Run a Python program

I created `hello.py` with one `print()` call. I ran it from the repository root and saw this message in Terminal:

```text
Hello from Python
```

### Task 4.2 — Compare compilers and interpreters

| Point | Compiler | Interpreter |
|---|---|---|
| When translation or execution happens | Translates source code into another form, often before the program runs. | Carries out program instructions at runtime. |
| Typical output | May produce an executable, object file or bytecode. | Produces the program's runtime results, such as text printed to Terminal. |
| One example | Clang can compile C source code into a native executable. | CPython executes Python bytecode. |
| One advantage | A compiled native executable can be run again without recompiling the source each time. | I can run a Python script directly with `python3` after editing it, without a separate build command. |

## 3. Commands / tools used

- A text editor to create and save `hello.py`.
- `python3 mission-04-programs/hello.py` to run the script.
- `print()` to display the message in Terminal.

## 4. My understanding

A compiler translates code into another form, such as machine code or bytecode. An interpreter carries out instructions while the program runs. Python can use both approaches in the same run. When I ran `hello.py`, CPython translated the source into bytecode and executed it, which displayed the message.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- `hello.py` contains the one-line Python program.
- `README.md` contains the observed output and the comparison table.

## 8. Commit details

- Commit message — `Compare compilers and interpreters`
- Push verification — See this file's **History** on GitHub for the published commit.