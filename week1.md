pwd  /// print working directory.

4 + 2 + 1 = read write execute

### Chapter: Exploring Basic Linux Commands and System Information


#### Section 1: Navigating the Linux File System and Using the `ls` Command

The Linux file system is organized hierarchically, with the forward slash (`/`) representing the **root directory**—the starting point of all paths. Notably, the root directory is unique in that it is its own parent; attempts to navigate to its parent directory leave you at root.

The `ls` command, fundamental for listing files and directories, offers a versatile syntax:

- **Options:** Short (`-l`, `-i`, `-d`, `-r`, `-t`) and their equivalent long forms (e.g., `--inode`, `--directory`).
- **Arguments:** File or directory names to specify the target of the command.
- The sequence of options is flexible; `ls -lid` and `ls -idl` produce identical outputs.
- The `-l` option provides a long listing format, showing detailed information including permissions, ownership, and timestamps.
- The `-d` option allows viewing directory details without listing their contents.
- The `-r` option enables recursive listing of directory contents.
- The `-i` option shows the **inode number**, a unique identifier for files.

**Key insights:**

- Using multiple slashes in file paths (`////usr///bin`) behaves identically to a single slash.
- Understanding inode numbers helps differentiate between files and their links.
- Long form options make commands more readable but are more verbose; short forms are preferred for quick, efficient command writing.

---

#### Section 2: Inspecting File Contents with Text Viewing Commands

Linux offers various commands to inspect the contents of text files, each suited to different purposes:

- **`less`**: A pager allowing scrolling through file content interactively, with the ability to quit anytime (`q`).
- **`cat`**: Concatenates and displays file content in one continuous stream without pagination; unsuitable for large files as it floods the terminal.
- **`more`**: Similar to `less` but with fewer features; allows viewing page by page.
- **`head`**: Displays the first ten lines by default, adjustable with the `-n` option to specify the number of lines.
- **`tail`**: Shows the last ten lines by default, also adjustable with `-n`.
- **`wc` (word count)**: Provides statistics on the number of lines, words, and bytes in a file. The `-l` option restricts output to line count only.

**Example used:**  
The file `/etc/profile`, a critical shell configuration file, is inspected with these commands to demonstrate their usage.

**Facts and figures:**

- The `/etc/profile` file had 27 lines, 97 words, and occupied 581 bytes.
- `head -n 5 /etc/profile` displays the


- **`whatis`**: Brief description, "whatis less" tells what less command do.. similarly **`whatis cat`** tells what cat command does.

- **`apropos`**: prints all the commands and thier description which contains keyword. **apropos who** lists all the command which contaions who keyword.
  
- **`man`**: . It provides detailed documentation on how to use a specific command or utility, including its syntax, options, and usage examples.  ex: **man who** lists all the description of what who command does.
- 
