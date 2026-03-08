# OpenCode Setup Guide

## How to Install OpenCode

### macOS (using Homebrew)

```bash
brew install opencode
```

### Other platforms

Visit the official documentation at https://opencode.ai for installation instructions.

## How to Install GitHub CLI (gh)

### macOS (using Homebrew)

```bash
brew install gh
```

### Verify installation

```bash
gh --version
```

## How to Login with gh CLI

1. Run the authentication command:
   ```bash
   gh auth login
   ```

2. Follow the prompts:
   - Select **GitHub.com**
   - Select **HTTPS** as the protocol
   - Select **Login with a web browser**
   - Copy the one-time code shown in the terminal
   - Authorize the application in your browser

3. Verify you're logged in:
   ```bash
   gh auth status
   ```

## Additional Resources

- OpenCode documentation: https://opencode.ai/docs
- GitHub CLI documentation: https://cli.github.com
