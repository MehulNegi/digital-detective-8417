# Mission 5 — Numbers and data

## 1. Task / objective

Convert numbers between decimal, binary and hexadecimal by hand. Verify the results in Python, build a small number converter and explain how computers represent text.

## 2. Work completed

### Task 5.1 — Manual conversions

For decimal-to-binary conversions, I divided by 2 repeatedly and read the remainders in reverse order.

| Conversion | Working | Answer |
|---|---|---|
| Decimal 13 to binary | 13 ÷ 2 = 6 remainder 1 → 6 ÷ 2 = 3 remainder 0 → 3 ÷ 2 = 1 remainder 1 → 1 ÷ 2 = 0 remainder 1. Read the remainders upwards. | `1101` |
| Decimal 25 to binary | 25 ÷ 2 = 12 remainder 1 → 12 ÷ 2 = 6 remainder 0 → 6 ÷ 2 = 3 remainder 0 → 3 ÷ 2 = 1 remainder 1 → 1 ÷ 2 = 0 remainder 1. Read the remainders upwards. | `11001` |
| Binary 1010 to decimal | 1×8 + 0×4 + 1×2 + 0×1 = 8 + 2. | `10` |
| Binary 1101 to decimal | 1×8 + 1×4 + 0×2 + 1×1 = 8 + 4 + 1. | `13` |
| Hexadecimal A to decimal | A has the value 10. It is in the ones place, so 10×1 = 10. | `10` |
| Hexadecimal 1F to decimal | F has the value 15. The 1 is in the sixteens place, so 1×16 + 15×1 = 31. | `31` |
| Binary 1111 to hexadecimal | 1×8 + 1×4 + 1×2 + 1×1 = 15. The hexadecimal digit for 15 is F. | `F` |

### Task 5.2 — Python verification

| Python expression | Result | Matches my working? |
|---|---|---|
| `bin(13)` | `'0b1101'` | Yes |
| `bin(25)` | `'0b11001'` | Yes |
| `int("1010", 2)` | `10` | Yes |
| `int("1101", 2)` | `13` | Yes |
| `int("A", 16)` | `10` | Yes |
| `int("1F", 16)` | `31` | Yes |
| `hex(15)` | `'0xf'` | Yes, 15 is F in hexadecimal. |
| `hex(31)` | `'0x1f'` | Yes, converting 31 back gives 1F. |
| `hex(int("1111", 2))` | `'0xf'` | Yes, binary 1111 is F in hexadecimal. |

Python includes `0b` before binary digits and `0x` before hexadecimal digits. It uses lowercase letters in `hex()` output, so `0x1f` represents the same value as hexadecimal `1F`.

### Task 5.3 — Number converter

The program reads a value with `input()`. Since `input()` returns text, I use `int()` to turn that text into a decimal integer. `bin()` returns the binary representation as a string, and `hex()` returns the hexadecimal representation as a string. The program displays both with `print()`.

| Test input | Binary output | Hexadecimal output |
|---|---|---|
| `13` | `0b1101` | `0xd` |
| `25` | `0b11001` | `0x19` |
| `31` | `0b11111` | `0x1f` |

### Task 5.4 — Text encoding

| Character | ASCII decimal code |
|---|---|
| `A` | `65` |
| `a` | `97` |

An encoding gives computers a standard way to represent characters as bytes. Using the same encoding when reading the bytes lets a program recover the original text. The rupee symbol `₹` is outside basic ASCII and can be encoded using UTF-8.

## 3. Commands / tools used

- `python3` opened the interactive Python prompt.
- `python3 mission-05-numbers-data/number_converter.py` ran the converter from the repository root.
- `input()`, `int()`, `bin()`, `hex()` and `print()` read, converted and displayed the values.
- `ord()` checked the numeric character codes for `A` and `a`.

## 4. My understanding

The same number can be written with different digits depending on its base. For example, 13 in decimal is 1101 in binary and D in hexadecimal. Encoding does a different job. It gives characters a consistent representation so a computer can save and read text.

## 5. Difficulties faced

No major difficulties.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

- `number_converter.py` asks for a decimal integer and prints its binary and hexadecimal representations.
- `README.md` contains my manual conversion steps, Python checks, converter test results and text-encoding notes.

## 8. Commit details

- Commit message — `Build and test the number converter`
- Push verification — See this file's **History** on GitHub for the published commit.