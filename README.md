# what-commit

Creates a commit from [whatthecommit.com](http://whatthecommit.com/), with flag support.

## Installation

```bash
mkdir -p ~/.local/bin # Create folder if it doesn't exist. 
# You're free to save the file anywhere you want, this is just standard
wget -O ~/.local/bin/whatcommit https://raw.githubusercontent.com/l1ving/what-commit/master/whatcommit
chmod +x ~/.local/bin/whatcommit
# Make sure ~/.local/bin is in your $PATH
# Source your shell if unsure
```

## Usage

```bash
whatcommit # Commit all added files
```

```bash
whatcommit -a # Commit all added files, supports git flags.
whatcommit -an # Commit all added files with the --no-verify flag
whatcommit "-a --cleanup=strip" # Commit all added files and strip whitespace from file
```

```bash
whatcommit -f uwu.txt # Commit only "uwu.txt". -f is a custom flag, and will not be passed to git.
```
