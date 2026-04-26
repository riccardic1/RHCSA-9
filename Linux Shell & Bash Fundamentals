🐧 Linux Shell & Bash Fundamentals
📂 Basic Commands
ls -l /etc      # Long listing of /etc
ll              # Alias for ls -l
alias           # Show current aliases
Common ls Options
ls        # List directory contents
ls -a     # Include hidden files (starting with .)
ls -l     # Long listing format
ls -h     # Human-readable sizes
ls -i     # Show inode numbers
ls -r     # Recursive listing
ls -t     # Sort by newest first
Navigation
cd        # Go to home directory
pwd       # Show current directory
⚙️ Internal vs External Commands
Internal Commands: Built into the shell (faster)
External Commands: Executable files on disk (slightly slower first run)
How Bash Resolves Commands
Checks if command is internal
If not, searches directories in $PATH
Useful Tools
type pwd     # Check if command is internal, external, or alias
which ls     # Show path of executable

type is more powerful than which because it also detects aliases and internal commands.

🛣️ The $PATH Variable
Defines directories where executables are searched
Does not include current directory (.) for security reasons
Run a script from current directory:
./script.sh
🔁 I/O Redirection
Standard Streams
Stream	Descriptor	Default
STDIN	0	Keyboard
STDOUT	1	Screen
STDERR	2	Screen
Redirectors
>       # Overwrite output
>>      # Append output
2>      # Redirect errors
2>&1    # Merge STDERR with STDOUT
<       # Redirect input
Examples
ls > output.txt
ls >> output.txt
ls invalid > out.txt 2>&1
Special Devices
/dev/null → Discard output
/dev/sda → Hard disk
/dev/tty1 → Terminal
🔗 Pipes

Use output of one command as input for another:

ls | less
history | grep cat
Commands run in parallel
Enables powerful chaining
🕘 Bash History
Stores last 1000 commands
File: ~/.bash_history
Commands
history             # Show history
history | less      # Paginated view
history | grep cat  # Search history
Shortcuts
Ctrl + r            # Reverse search
!number             # Run command by number
!text               # Run last command starting with text (⚠️ dangerous)
Manage History
history -d <num>    # Delete specific entry
history -c          # Clear current session
history -w          # Write cleared history to file
⚡ Bash Completion
Press Tab to auto-complete commands/files
Double Tab shows suggestions
📝 VIM Basics
Modes:
Command Mode
Insert Mode
vimtutor   # Interactive tutorial
🌍 Environment Variables
Basics
echo $LANG   # Show language
env          # List all variables
Example: LANG=en_US.UTF-8
Configuration Files
File	Purpose
/etc/profile	Global login config
/etc/bashrc	Global subshell config
~/.bash_profile	User login config
~/.bashrc	User subshell config
📢 Login Messages
/etc/motd → Message of the Day (after login)
/etc/issue → Message before login (CLI only)
📚 Finding Help
man ls              # Manual page
man -k keyword      # Search manuals
apropos keyword     # Same as man -k
command --help      # Quick help
Navigation in man
G → Bottom
/text → Search
Notes
mandb   # Update manual database

Additional docs:

/usr/share/doc
🔑 Key Terms
Shell: Interface to execute commands
Bash: Default Linux shell (e.g., RHEL)
Variable: Named value that can change
Internal Command: Built into shell
External Command: Executable file on disk
🧠 Tips
Use type over which for deeper inspection
Avoid using !text unless you're sure (executes immediately)
Use /dev/null when you want to suppress output
Remember: current directory is not in $PATH
