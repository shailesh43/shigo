# Shigo 

A lightweight, interactive shell implementation written in Go. This shell provides basic command-line functionality with modern features like tab completion and environment variable management.

## Features

### Core Functionality
- Interactive command-line interface
- Command execution with proper I/O handling
- Environment variable management
- Tab completion for commands and files
- Command history with arrow key navigation
- Signal handling (Ctrl+C, SIGTERM)

### Built-in Commands
- `cd` - Change directory (supports `cd` to home directory)
- `export` - Set environment variables
- `env` - Display current environment variables
- `exit` - Exit the shell

### Technical Features
- Pure Go implementation
- Concurrent signal handling using goroutines
- Robust command execution using `os/exec`
- Smart tab completion for files and built-in commands
- Command history navigation
- Graceful interrupt handling

## Installation

### Prerequisites
- Go 1.16 or higher
- Linux/Unix-based operating system

### Steps
```bash
# Clone the repository
git clone https://github.com/shailesh43/shigo.git

# Navigate to the project directory
cd shigo

# Install dependencies
go get github.com/c-bata/go-prompt

# Build the project
go build

# Run the shell
./shigo
```

## Usage

### Basic Commands
```bash
shigo~ ls                    # List files
shigo~ pwd                   # Print working directory
shigo~ cd /path/to/dir      # Change directory
shigo~ export VAR=value     # Set environment variable
shigo~ env                  # Show all environment variables
shigo~ exit                 # Exit the shell
```

### Environment Variables
```bash
# Set an environment variable
shigo~ export MYVAR=hello

# Use an environment variable
shigo~ echo $MYVAR

# View all environment variables
shigo~ env
```

### Features
- Use Tab for command and file completion
- Use Up/Down arrows to navigate command history
- Use Ctrl+C to interrupt running commands
- Use environment variables with $VARNAME syntax

## Current Limitations
- No shell scripting support
- No job control (background processes)
- No persistent command history
- Limited built-in commands compared to bash/zsh
- No alias support

## Dependencies
- [go-prompt](https://github.com/c-bata/go-prompt) - For enhanced terminal interaction
- Standard Go libraries

## Contributing
Contributions are welcome! Feel free to submit pull requests or open issues for bugs and feature requests.

## Future Enhancements
- [ ] Shell scripting support
- [ ] Job control (background processes)
- [ ] Persistent command history
- [ ] Additional built-in commands
- [ ] Alias support
- [ ] Pipeline support
- [ ] Input/Output redirection

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Inspired by traditional Unix shells
- Built with Go's standard library and go-prompt
- Special thanks to all contributors

## Author
[Shailesh Sathe]

## Project Status
This project is currently in development. Feel free to contribute or report issues.
