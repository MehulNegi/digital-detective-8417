# Mission 0 — Create your GitHub workspace

## 1. Task / objective

Set up the `digital-detective-8417` repository with a root README and a separate folder for each mission.

## 2. Work completed

I created nine mission folders and an `evidence/` folder. I added a README at the root and inside each mission folder. I also created an empty `number_converter.py` file for Mission 5.

## 3. Commands / tools used

- `python3 --version` showed Python 3.14.6.
- `git --version` showed Git 2.56.0.
- `mkdir` created the project and mission folders.
- `touch` created the empty files.
- `find . -maxdepth 2 -type f | sort` listed the files so I could check that all 11 were present.

## 4. My understanding

A Git repository stores my project files and tracks changes through commits. Giving each mission its own folder makes it easier to find the notes and files for that mission.

## 5. Difficulties faced

I tried to create the mission READMEs with `touch README.md mission-*/README.md mission-05-numbers-data/number_converter.py`. Zsh gave me a `no matches found` error because `mission-*/README.md` tried to match files that did not exist yet.

## 6. How I resolved them

I used `mission-*/` to match the folders that already existed. Then I used a loop to run `touch` on the `README.md` path inside each folder. I checked the result with `find` and saw all 11 expected files.

## 7. Evidence / files

- `README.md` in the repository root
- A `README.md` inside each of the nine mission folders
- `mission-05-numbers-data/number_converter.py`

## 8. Commit details

Commit message: `Set up Digital Detective mission structure`

GitHub push verification: Pending.