# Mission 3 — Understand the operating system

## 1. Task / objective

Explore macOS, running processes, storage, paths and file permissions. Explain what the operating system does when I use my computer.

## 2. Work completed

### Task 3.1 — System information

| Information explored | What it tells me | My observation |
|---|---|---|
| Operating system | Which OS is running and its version. | `sw_vers` showed macOS and displayed its version and build. |
| Current account | Which user account the Terminal commands are running under. | `whoami` printed the active account name. I recorded it as [redacted]. |
| Used and available storage | How much space is used and how much is available on the filesystem containing my assignment. | `df -h .` showed separate `Used` and `Avail` columns. |
| System activity | What the system is doing at the time of the check. | `top` showed a snapshot with information about processes and CPU activity. |

### Task 3.2 — Processes

A process is a running instance of a program. The PID is the number the operating system uses to identify that process while it is running. TextEdit and Finder are two examples. TextEdit lets me edit documents, and Finder lets me browse files and folders.

### Task 3.3 — Paths and permissions

At first, `pwd` showed that I was in `digital-detective-8417`. After I ran `cd mission-03-operating-system`, the path ended in `digital-detective-8417/mission-03-operating-system`.

An absolute path starts at the filesystem root. The absolute path to my Mission 3 folder has this form, with the private part redacted: `/[redacted]/digital-detective-8417/mission-03-operating-system`.

A relative path starts from the directory I am in. From the repository root, `mission-03-operating-system/README.md` is a relative path to this file.

I used `ls -l` to inspect `practice.txt` from Mission 2. The owner's permission characters were `rw-`. The owner can read and write the file. The dash in the third position means execute permission is absent.

| Permission | Meaning | Example |
|---|---|---|
| `r` | Read a file's contents. | Open `practice.txt` and see its text. |
| `w` | Write changes to a file. | Add another line to a text file. |
| `x` | Execute a file or traverse a directory. | Run an executable script directly. |

### Task 3.4 — Operating-system responsibilities

| Responsibility | What the OS does | Example |
|---|---|---|
| Process management | Starts and stops processes and schedules their work on the CPU. | TextEdit and Finder can both run while I work. |
| Memory management | Allocates memory to programs and manages how they use RAM. | TextEdit uses memory to hold the document I am editing. |
| Device management | Coordinates access to hardware through drivers. | macOS passes keyboard input to the active application. |
| File management | Organises files and directories and handles reads and writes. | Saving a note creates a file I can reopen later. |
| User interface / shell | Provides ways to interact with the computer through windows and commands. | I can open a folder in Finder or enter it with `cd` in Terminal. |
| Security and permissions | Checks which users and processes can access files or perform operations. | File permissions determine whether an account can modify a file. |

## 3. Commands / tools used

- `sw_vers` and `whoami` to check the OS and active account.
- `df -h .` to inspect storage usage in readable units.
- `top`, `head`, `ps` and `grep` to inspect system activity and find processes.
- TextEdit to open an application for the process check.
- `pwd` and `cd` to observe how my working directory changed.
- `ls -l` to inspect the practice file's permissions.

## 4. My understanding

A process is the running program I can identify with a PID. A file path tells me where something is, and permissions tell me what an account can do with it. I used all three ideas when I checked which programs were running, moved into the Mission 3 folder and inspected the permissions on my practice file.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- `README.md` contains my system observations and tables.
- `../mission-02-terminal/terminal-practice/practice.txt` is the existing file I inspected for permissions.

## 8. Commit details

- Commit message — `Document operating system and file management`
- Push verification — See this file's **History** on GitHub for the published commit.