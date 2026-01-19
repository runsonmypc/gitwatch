# gitwatch

A minimal, real-time git status monitor for your terminal.

![gitwatch demo](demo.png)

## Features

- **Branch + sync status** - Shows current branch with ↑/↓ for ahead/behind remote, ✓ when synced
- **Last commit** - Hash, message, and relative time
- **Staged changes** - Files staged for commit with line counts
- **Unstaged changes** - Modified tracked files with line counts
- **Untracked files** - New files with line counts
- **Compact summary** - Total files changed, insertions, deletions, new files

## Requirements

- `watch` command (`brew install watch` on macOS)
- Git
- Bash

## Installation

```bash
# Clone the repo
git clone https://github.com/yourusername/gitwatch.git

# Copy to your bin directory
cp gitwatch/gw ~/bin/gw
chmod +x ~/bin/gw

# Make sure ~/bin is in your PATH
echo 'export PATH="$HOME/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

## Usage

Run `gw` in any git repository:

```bash
cd your-project
gw
```

Best used in a narrow terminal pane alongside your editor. Updates every second.

Press `q` to quit.

## Example Output

```
feat/my-feature ↑2
a1b2c3d Add user authentication (2 hours ago)

○ unstaged
 src/auth.py      |  45
 src/middleware.py |  12

◌ untracked
 tests/test_auth.py |  30

  2Δ  +57  -0   1 new
```

## License

MIT
