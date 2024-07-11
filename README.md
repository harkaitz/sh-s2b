# S2B - Shell to batch

Pack shell scripts written for Busybox for Windows in batch files.

## Help

dialog-w

    Usage: dialog-w [DIALOG-CMDS...]
    
    Wrapper around dialog(1) for windows. This script downloads dialog
    if needed and executes it. When sourced it provides:
    
      dialog_clear   : Clear screen.
      dialog_SEL ... : Execute dialog, save result in SEL.
      dialog ...     : Execute dialog.

s2b

    Usage: s2b OPTS... SCRIPT ARGS...
    
    Create a SCRIPT.bat file from a shell script for easy sharing
    with other MS Windows users.
    
    Notes:
    
      1. When a shell is missing a busybox 64 bits shell is downloaded.
      2. The shell is installed in "%LOCALAPPDATA%\Microsoft\WindowsApps".
      3. The capability of downloading other programs other than "sh.exe"
         was left out knowingly. That should be done by the script.
    
    Command line arguments:
    
      -o DIR : Output directory (by default ~/S2B).
      -i     : Automatically install script in PATH on execution.
      -e     : Open bundle directory with "explorer.exe" after creation.
      -p     : Put a pause after the execution.
    
    Example: s2b -eip s2b_example HELLO WORLD

s2b_example

    Usage: s2b_example ARGUMENTS...
    
    This is a sample script for s2b, it prints a message and quits. Build
    a wrapper for this script with "s2b -eip s2b_example".

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
