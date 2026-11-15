# Mission 2 — Become comfortable with the Terminal

## 1. Task / objective

Practise navigating folders, creating and managing files, using command options and pipes, and understanding what a package manager does.

## 2. Work completed

### Task 2.1 — Basic Terminal operations

| Operation / command | What it does | What I observed |
|---|---|---|
| `pwd` | Prints the full path of the current directory. | The path ended in `digital-detective-8417` when I was at the repository root. |
| `ls` | Lists visible files and folders in the current directory. | I could see `README.md` and mission folders such as `mission-02-terminal`. |
| `ls -l` | Shows a detailed directory listing. | I could see information such as permissions, sizes and modification dates. |
| `cd ..` | Moves up to the parent directory. | I left `mission-02-terminal` and returned to `digital-detective-8417`. Running `pwd` confirmed the change. |
| `mkdir terminal-practice` | Creates a new directory. | It created `terminal-practice` inside `mission-02-terminal`. |
| `touch original.txt` | Creates an empty file when the file does not already exist. | `original.txt` appeared in the practice folder. |
| `cp original.txt copied.txt` | Creates a copy with a different name. | Both `original.txt` and `copied.txt` existed after the copy. |
| `mv copied.txt renamed.txt` | Changes the name of the copied file. | The copy appeared as `renamed.txt`, and `original.txt` was still there. |
| `cat original.txt` | Prints a file's contents. | The command printed nothing because the file was empty. |

### Task 2.2 — Writing and backing up a file

I used `>` to write the first line to `practice.txt` and `>>` to add the second line. When I ran `cat practice.txt`, it displayed:

```text
This is my first line.
This is my second line.
```

I used `cp practice.txt backup.txt` to make a backup and `mv backup.txt practice-backup.txt` to rename it. The original two-line file was still saved as `practice.txt`.

### Task 2.3 — Flags and pipes

`ls` showed the names of visible entries. `ls -lah` showed extra details such as file permissions and sizes. The `-l` flag selected the detailed format, `-a` included hidden entries such as `.` and `..`, and `-h` made the sizes easier to read.

In `ls -l | head -n 3`, `ls -l` produced the detailed listing. The pipe `|` passed that output to `head -n 3`, which displayed only the first three lines.

### Task 2.4 — Package managers

Homebrew is a package manager for macOS. A package manager makes it easier to install, update and remove software from one place. It can also track installed packages and manage dependencies that those packages need.

## 3. Commands / tools used

- `pwd`, `ls` and `cd` to check my location, inspect directories and move between them.
- `mkdir` and `touch` to create the practice folder and an empty file.
- `cp`, `mv` and `cat` to copy, rename and read files.
- `printf` with `>` and `>>` to write text and append another line.
- `ls -lah` and `ls -l | head -n 3` to inspect a detailed listing and limit its output.
- `command -v brew` to check whether Homebrew was available.

## 4. My understanding

`pwd` tells me exactly which directory I am working in. `ls` helps me check what is inside that directory before I work with its files.

`>` replaces a file's contents, while `>>` adds text at the end. `cp` leaves the source file in place and creates a separate copy. `mv` changes a file's name or location. Flags change how a command runs, and a pipe lets one command use another command's output.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- `terminal-practice/original.txt` — the empty file I created.
- `terminal-practice/renamed.txt` — the copy after renaming it.
- `terminal-practice/practice.txt` — the file with both lines.
- `terminal-practice/practice-backup.txt` — the renamed backup of the two-line file.

## 8. Commit details

- Commit message — `Complete Terminal and file management mission`
- Push verification — See this file’s **History** on GitHub for the published commit.