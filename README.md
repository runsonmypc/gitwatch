# gitwatch

Real-time git status monitor for your terminal.

![gitwatch demo](demo.png)

## Features

- Branch with sync status (✓ synced, ↑N ahead, ↓N behind)
- Staged / unstaged / untracked files with line counts
- Smart path truncation at directory boundaries
- Compact summary: `2Δ +57 -3 1 new`
- Last 3 commits with auto-truncation to fit terminal width

## Install

```bash
brew install watch  # macOS only
git clone https://github.com/runsonmypc/gitwatch.git
cp gitwatch/gw ~/bin/
chmod +x ~/bin/gw
echo 'export PATH="$HOME/bin:$PATH"' >> ~/.zshrc
```

## Usage

```bash
gw  # run in any git repo, q to quit
```

## License

MIT
