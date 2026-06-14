# Relational Databases & Developer Environments (v9): Master Course Manual

This comprehensive engineering textbook bundles all foundational computing skills—covering code editors, terminal systems architectures, remote Git collaboration methodologies, and production-grade Relational Database Design.

---

## Module 1: Developer Environment & Local Workspaces

### Lecture 1.1: What Is A Code Editor And Ide

# What Is a Code Editor and IDE?

You might think these are the same thing, but not quite. A code editor is any application that allows you to edit code files. An IDE, or Integrated Development Environment, is a full application that allows you to compile, run, and debug your code while you edit it.

Perhaps some examples might be helpful.

First, let's consider a few popular IDEs. Visual Studio is an integrated development environment by Microsoft that provides a comprehensive suite of tools for building, debugging, and deploying applications across various platforms.

Another IDE is XCode. Xcode is an integrated development environment by Apple designed for creating, coding, and debugging applications for macOS, iOS, watchOS, and tvOS.

And another IDE would be Android Studio. Android Studio is an integrated development environment by Google specifically designed for building, debugging, and testing Android applications.

Those are just a few examples of IDEs. Now, let's take a look at a few popular code editors.

Visual Studio Code is a lightweight, open-source code editor by Microsoft that supports a wide range of programming languages and provides features like debugging, syntax highlighting, and version control through extensions.

Another popular editor would be Sublime Text. Sublime Text is a fast, versatile text editor known for its sleek interface, powerful features, and support for a wide range of programming languages through customizable syntax highlighting and plugins.

And another one is Notepad++. This is a free, open-source, text and source code editor for Windows that offers syntax highlighting, code folding, and a range of plugins to enhance productivity and customization.

You may have noticed how the code editors focus primarily on the text contents of the file, where the IDEs expose various tools to manage your code.

These examples are all local programs you can run on your computer, but there are also cloud-based editors that you can use.

A cloud-based editor is an online tool that allows users to write, edit, and manage code or text directly through a web browser without needing to install software locally.

Let's take a look at a few cloud-based editors.

Replit is an online platform that provides a collaborative environment for coding, allowing users to write, run, and share code in various programming languages directly from a web browser.

Another popular cloud-based editor is GitHub Codespaces. This is a cloud-based development environment that provides instant access to a fully-configured code editor and development tools directly from GitHub, enabling seamless coding and collaboration.

And another one is Ona. Ona is a cloud-based development environment that integrates with GitHub and GitLab, offering instant, customizable workspaces for coding, building, and debugging directly from your browser.

And there are many more options. Some options, such as Visual Studio Code, are highly extensible and can work with multiple different project types and languages. Other options might be specifically tailored to a small subset of languages or project types.

The application you use might be different for specific projects. You should explore the options to see what will work best for your needs.

---

### Lecture 1.2: How To Install Visual Studio Code Onto Your Computer

# How to Install Visual Studio Code onto Your Computer

To install VS Code, you'll want to visit their website to get the appropriate installer for your operating system. Make sure you visit the VS Code website, and not the Visual Studio website.

For Windows, you can download an EXE installer. Once you've downloaded it, run the file and the setup wizard will take you through the installation process.

For Mac, you can download a zip archive which contains a `.app` that you can run. You can also install VS Code via homebrew.

Open up the Terminal app on your Mac and run the following command:

```
brew install --cask visual-studio-code
```

On Linux, you can download a `.deb` or `.rpm` file directly. Once you have it installed, you can use the appropriate executable, or CLI command (typically `code`), to launch the application. And now you're ready to code.

---

### Lecture 1.3: How To Create A Project And Run Your Code Locally In Vs Code

# How to Create a Project and Run Your Code Locally in VS Code

To get started, you should know that VS Code considers projects to be "workspaces". The workspace is whichever directory you opened in VS Code.

To begin, you will need to use a command line interface to create a new directory for your new project. A directory is another name for the folder.

Command-line interfaces, or CLI for short, allow you to interact with your operating system through text-based commands. You will learn more about these tools in future lessons.

If you are on Windows, you can use the Command Prompt or PowerShell. If you are on a Mac, you can open up your Terminal app.

Once the command line is open, navigate to the home directory by typing in the `cd ~` command and hitting `enter` on your keyboard. Then type in the `mkdir my-project` command and hit `enter`. `mkdir`, or "make directory" is the command used to create a new directory. You should then open your new directory with VS Code.

There are also some other graphical ways to create a new directory.

Depending on your operating system, you might have a context menu (or right-click option) to open VS Code directly from your file explorer. You could also choose to double-click on the VS Code application. If you feel comfortable with the command line you can run the command `code /path/to/folder`.

Once it's open, you should see a new blank workspace.

To create a new file, click on the `File` menu at the top-left corner and select `New File...`. Then name your file `index.html` and click on `Save`.

Now you should see your new file in the explorer tab. Try adding some HTML to your `index.html` file.

Now you might be tempted to open the HTML file in your browser directly. While that can work, it can also lead to all sorts of unexpected bugs, such as CSS not loading properly.

Instead, you should put your HTML file behind a proper web server. That can sound like an intimidating task if you are new to coding, but there's actually a way to do this right from VS Code.

You'll need to grab the *Live Server* extension first, which is available for free in the marketplace.

Click on the extensions tab in the left hand corner and type in `Live Server` in the search bar.

Once you have this installed, you should see a `Go live` button in your status bar. Make sure you have your HTML file open, and then click it.

Your new page should open automatically in a new tab in the browser. If it doesn't then you can go directly to `http://localhost:5500/`

Congratulations! You've now set up your very own project in VS Code, and can view your changes with live server.

---

### Lecture 1.4: What Are Some Good Vs Code Extensions You Can Use In Your Editor

# What Are Some Good VS Code Extensions You Can Use in Your Editor?

*Better Comments* is an extension that offers special highlighting for specific code comments. For example, it will call out "TODO" comments, as well as syntax to indicate questions or warnings.

*Code Spell Checker* offers indication when you have spelled something incorrectly in your code. Because it is designed for code files, it will account for things like camel case.

*Error Lens* will help you catch any highlighted errors in your code. Rather than having to rely on the underline that VS Code shows by default, this extension highlights the entire line and displays the error message.

*Indent Rainbow* adds color to your different levels of indentation. In combination with VS Code's native bracket pair colorization, this can dramatically help identify what scope your code is in.

Or maybe you're looking for something a bit more practical? Consider an AI assistant, like *GitHub Copilot* or *Tabnine*, to offer you inline suggestions as you are writing your code.

An icon pack, such as *VS Code Great Icons*, can help make your file tree cleaner and easier to parse at a glance. And an extension like *Colorize* can help you understand the values in your CSS properties.

You'll also want language-specific extensions for your projects. If you are using JavaScript, you will likely want *ESLint* and *Prettier* to lint and format your code. If you are using TypeScript, you might want *Pretty TypeScript Errors* for easier to read messages.

Finally, you can also have a bit of fun with your editor. *VS Code Pets* offers configurable virtual pets to keep you company while you squash some bugs.

*Power Mode* will create flashy effects when you achieve a high enough "combo" by writing more code.

*Discord Presence* will let you show off what you're working on to all of your friends.

And there are so many more extensions out there. Feel free to explore the extension marketplace and see what works best for you.

---

### Lecture 1.5: What Are Several Useful Keyboard Shortcuts For Maximizing Productivity In Vs Code

# What Are Several Useful Keyboard Shortcuts for Maximizing Productivity in VS Code?

You're likely already familiar with some of the basic shortcuts, which are inherited from your operating system. Shortcuts like `Ctrl + S` to save, `Ctrl + C` to copy, and `Ctrl + V` to paste all work in VS Code.

But there's a few that are application specific and can still level up your productivity. It's worth noting that some of these shortcuts may differ by operating system.

For example, `Shift + Alt + F` will run your configured formatter (such as prettier, for a JavaScript project) on the currently opened file.

Or `Ctrl + Shift + F` (Windows), or `Cmd + Shift + F` (Mac), to search the text contents of all the files in your workspace. Then `Ctrl + Shift + H` (Windows), or `Cmd + Shift + H` (Mac), if you want to run a find-and-replace.

If you need to remove a line, `Ctrl + Shift + K` (Windows), or `Cmd + Shift + K` (Mac), will delete it.

Need some extra room for all your code? `Ctrl + B` (Windows), or `Cmd + B` (Mac), will hide the sidebar - which has the file list and extensions menu.

Or maybe you just can't see your code? `Ctrl + plus` (Windows), or `Cmd + plus` (Mac), will increase the scaling of the editor, and `Ctrl + minus` (Windows), or `Cmd + minus` (Mac), will decrease it.

Another helpful feature in VS Code is multi-line editing, which allows you to make changes across several lines at once. For example, you can place multiple cursors by using `Ctrl + Alt + down` and `Ctrl + Alt + up` (Windows/Linux), or `Option + Command + down` and `Option + Command + up` (Mac), to extend the cursor to consecutive lines. You can also press and hold `Alt` (Windows/Linux) or `Option` (Mac) and click to add cursors on separate lines wherever you need them. Once the cursors are placed, anything you type or delete will apply to all those locations simultaneously — which can save a lot of time when working with repetitive code.

Finally, if you forget any of these shortcuts, you always have `Ctrl + Shift + P` (Windows), or `Cmd + Shift + P` (Mac), which opens the command palette for you to select whatever you may need.

With this knowledge, and maybe a little practice, you are well on your way to becoming a VS Code power user.

---

## Module 2: The Command Line & Bash Essentials

### Lecture 2.1: What Is The Terminal And How Does It Differ From The Command Line

# What Is the Terminal, and How Does It Differ from the Command Line?

Let's learn about the terminal, and how it differs from the command line.

The command line is a basic text input interface which allows a user to enter "commands", usually in the form of a series of characters, and submit or execute them, usually by pressing the "Enter" key. You will most-commonly see command line interfaces within a terminal.

A terminal is a special application that offers a command line interface to perform system-level commands beyond the basic read/write operations. You may also hear about "terminal emulators", which are essentially applications that wrap a basic terminal interface to offer additional features or functionality. But for most general purposes, you are probably safe to refer to these as "terminals" as well.

Finally, we will also need to talk about "shells". A shell is the software that wraps the command line and interprets your inputs as commands, returning the output.

But how can you access the terminal on your system?

Well, if you are running a modern version of Windows, you will likely have two different options. Windows offers two distinct shell applications out of the box: Powershell and Command Prompt.

Both of these shells come with their own terminal applications (which share the name of the respective shell), so you can use your application menu to start either a Powershell terminal or a Command Prompt terminal.

Windows also offers a relatively new and modernized terminal emulator aptly named Microsoft Terminal.

You can install this application from the Windows Store, and are then able to launch it just like you would your Powershell or Command Prompt terminals. The advantage of the Microsoft Terminal is that it allows you to access both the Powershell and Command Prompt shells from the same application, as well as your respective Linux shell if you have configured Windows Subsystems for Linux.

MacOS offers a terminal that is aptly named "Terminal". You can access this through your spotlight search, or through your application launcher.

MacOS also offers support for third-party terminal emulators, such as iTerm or Ghostty. You can install these applications from their home pages.

On Linux, the default terminal (and how you launch it) depends highly on the distro and desktop environment you use. There's a lot of support for third-party terminal emulators, too. For example, you could set up kitty in Arch Linux - and you can launch it with an application manager such as wofi.

Linux arguably has the largest variety of terminal applications to choose from. Most of these can be installed through your distro's package manager.

The distinction between "terminal", "shell", and "command line" may seem rather pedantic at times. And for the most part, the terms can generally be used interchangeably. But it is important to know that they have specific meanings, and what each of those meanings are.

---

### Lecture 2.2: What Is Bash And What Are Some Bash Commands

# What Is Bash, and What Are Some Basic Commands?

Let's learn about Bash and some of its basic commands.

Bash stands for Bourne Again SHell, and is arguably the most common shell you will encounter in Unix-like environments. As such, it can be very beneficial to understand how to navigate this shell and use the common commands.

The first command is `pwd`, which prints the current working directory to the terminal. The "working directory" refers to the directory the terminal is currently pointed at, which is an important thing to know for many of these other commands.

It is entirely possible that your terminal is pointed to the wrong directory. The `cd` command allows you to change directories. You can specify an absolute path, prefixed with a forward slash (`/`), a relative path with no prefix, and use the double-dot (`..`) syntax to move up to the parent directory.

The next command is `ls`, which lists the contents of your current working directory. This is helpful to see if a file or folder exists in your directory. The `ls` command also takes flags to show hidden files (the `-a` flag), file permissions (the `-l` flag), and other features. You will learn more about command flags in the next lesson. You can also use `less` or `cat` to view the contents of a file.

What if the directory does not contain the file or folder you need? There are commands called `mkdir` and `touch` that allow you to create them. `mkdir` creates a new directory, or folder, and `touch` creates a new file. Both of these commands accept the name of the file or folder you want to create. For example, `touch readme.md` creates a new Markdown file named `readme.md`.

Maybe your new file should not have been named `readme.md`, but it should have been `readthis.md`. Thankfully, the `mv` command allows you to move (or rename) a file. It takes the old file name and the new file name.

The `rm` command allows you to remove (or delete) a file, and with the `-r` flag will delete a directory. Sometimes a file might be protected, and you'll need to include the `-f` flag.

The `cp` command can be used to copy a file or directory to a new location. Unlike the `mv` command, the `cp` command does not remove the original file - and in order to copy a directory, you'll need to pass the `-r` flag.

The `echo` command can be thought of as the Bash equivalent of a `console.log()` or `print()` function. `echo` takes a string argument, wrapped in quotes, and prints it to the terminal. This might seem silly to run in the terminal, just to get text back in the terminal, but you can actually chain `echo` to a control symbol. The `>` symbol allows you to specify a filename to create or overwrite with the new string, like `echo "Naomi was here." > readme.md`, and the `>>` symbol will append to the file.

There are many more Bash commands available to you, such as `head`, `tail`, `chown`, and `chmod`. It would be impossible to cover them all in this lesson. But you can use the `man` command to see the manual or help page for nearly any command.

You'll likely remember the commands you use most frequently. And for the rest, you can always check the man page.

---

### Lecture 2.3: What Are Some Command Options And Flags

# What Are Some Command Options and Flags?

Let's learn about command options and flags.

In a previous lesson, you learned about passing arguments to commands such as `touch readme.md`. Options, or flags, are special arguments you can pass to a command that affect the way it behaves. The two terms are used interchangeably, though "flags" tends to be used more specifically for options that serve as an on/off toggle.

Options are typically prefixed with one or two hyphen (`-`) symbols, which helps provide a visual distinction between an option and an argument. First, let's look at the two-hyphen, or "long form", syntax.

Many applications, such as `ls`, accept a `--version` flag, which prints the current version of the application to the terminal instead of running the application's commands.

Many applications also offer a `--help` flag, which prints instructions on how to use the application.

The one-hyphen, or "short form", syntax typically uses options that are a single letter. For example, the `-a` flag with `ls` lists all files, including hidden files that start with a dot (`.`), like `.env`.

The advantage of these short options is that you can chain multiple flags together. Instead of `ls --all --human-readable --size` you can use the single letters all at once with `ls -ahs`.

Some options expect a value to be passed to them.

When using long-form options, you typically need to use an equal sign. In this syntax, the value is directly concatenated to the option with the equal (`=`) symbol. Here is an example of modifying the behavior of `ls` to either include or exclude colors:

```
ls --color=never
```

When using short-form options, you typically separate the value with a space. For example, here are the long and short form options for setting the `width` of the `ls` result:

```
ls -w 50
```

```
ls --width=50
```

Notice how the short form uses `-w 50`, while the long form uses `--width=50`. This distinction is important to know, to avoid passing an option value as a positional argument instead.

But if you are ever unsure, remember you can usually use the `--help` flag to see the expected syntax for options!

---

### Lecture 2.4: What Are Some Shortcuts You Can Use In The Command Line To Speed Up Productivity

# What Are Some Shortcuts You Can Use in the Command Line to Speed Up Productivity?

Let's learn about command line shortcuts you can use to speed up productivity.

Terminal and command line shortcuts can help you streamline your workflows and maximize your productivity. For Linux and macOS, which can both trace their roots to Unix, many of these shortcuts will be the same. But for Windows, there will be some differences.

The first shortcut is the up arrow key. Pressing this key will allow you to cycle backwards through your command history, one command at a time. The down arrow key, then, can be used to cycle forwards through your command history. These two keys allow you to quickly cycle through the commands you have previously run to find one you need to run again.

Many shells will also offer an auto-complete feature, proposing commands based on what you have started to type. The tab key can be used to fill in the rest of the suggestion, quickly populating your command line with the full syntax. How these suggestions are generated will vary from shell to shell. For example, in zsh these suggestions are based on your most recent command history. But in PowerShell, they are based on commands, variables, and arguments that are available (with less weight on how recently they were used).

Sometimes a command may result in a lot of output on your terminal. This extra noise can get in the way, or become disruptive to your workflow. In \*nix based terminals found on Linux and macOS devices, you can press Control + L to clear the entire screen and start with a fresh clean prompt. In PowerShell, you would need to run the `cls` command (which you can bind to a key combination like Control + L).

If you need to interrupt a command to stop its execution, you can use Control + C to kill the process. This will terminate the command and create a new prompt, allowing you to continue with whatever else you may need to work on. For PowerShell users, Control + C is also used to copy text - and will only work to terminate a process when the context is not ambiguous (such as when there is no text selected to copy).

The next couple of shortcuts are only available in \*nix based terminals, and do not have a PowerShell alternative.

There may be times when you need to multitask, allowing a process or command to run in the background while you work on another. Pressing Control + Z places the current process in a background task and returns you to the command line, where you can continue your work. When you need to shift focus back to the background task, you can use `fg` to restore it.

And finally, there may be commands you need to run twice in a row. You can press the up arrow key to cycle backwards to the previously run command, but you can also type two exclamation points (`!!`) into the command line and hit enter - this will automatically run the last executed command.

Many terminals offer even more shortcuts, and I encourage you to read the documentation for your particular setup to find the shortcuts that work best for you. But these basic universal shortcuts should serve as a great starting point for maximizing your productivity and becoming a terminal wizard.

---

### Lecture 2.5: What Is Nano

# What Is Nano?

When working in the terminal, standard text editors aren't always available, but there are programs designed to edit files directly from within the terminal.

Linux environments typically include a text editor. Vi, or Vim, tend to be the most common. Emacs and Nano may need to be installed manually, but they are readily available for nearly every distribution.

The challenge with Vim is it has a substantial learning curve. If you are not already familiar with it, you may not even know how to close the application! Emacs is arguably a bit more user friendly, but still has its own tome of keyboard shortcuts.

Nano is considerably more streamlined and user-friendly, especially for new learners. It can be much quicker to dive in and edit a file with Nano, and the application even offers on-screen help for the basic keyboard shortcuts.

The tradeoff for this, however, is the lack of extensibility. Unlike Vim or Emacs, which can be extended with plugins to become full development environments, Nano is rather barebones.

Let's take a peek at what Nano can do. To open a file, you can enter `nano <filename>` in the terminal.

Once a file is open, you will see the version of Nano you are running and the name of the file you have open at the top of the screen.

Below that is the content of the file. You can use the arrow keys to navigate your cursor and insert or delete text with your keyboard. The file will scroll as needed to follow.

Then, at the bottom, you will see a list of available keyboard shortcuts, that looks something like this:

```
^G Help   ^O Write Out    ^F Where Is   ^K Cut      ^T Execute  ^C Location     M-U Undo    M-A Set Mark    M-] To Bracket    M-B Previous
^X Exit   ^R Read File    ^\ Replace    ^U Paste    ^J Justify  ^/ Go To Line   M-E Redo    M-6 Copy        ^B Where Was      M-F Next
```

Shortcuts which start with the caret (`^`) symbol indicate you need to hold the Ctrl key and press the indicated letter. Shortcuts which start with `M-` require you to hold the "meta key", which in most setups should be the Alt key, and press the letter.

To edit a file in Nano, you only need to know a few of the shortcut commands. After making changes to a file, you can press `Ctrl + O` to "Write Out", or save, the file. After entering the command, you will see the menu at the bottom change to this:

```
File Name to write : <filename>
^G Get Help                 ^T  To Files
^C Cancel                   TAB Complete
```

Press enter to save the file and go back to editing the file, or `Ctrl + C` to cancel and go back to editing the file.

While in the editor, you can press `Ctrl + X` to exit Nano and go back to the terminal. If you have unsaved changes when trying to exit, you will see this in the bottom menu:

```
Save modified buffer (ANSWERING "No" WILL DESTROY CHANGES) ?
                            Y Yes
^C Cancel                   N No
```

Press `Y` to save your unsaved changes, or `N` to discard them.

With this knowledge, you should be better prepared the next time you need to quickly edit a file on a remote server, where you might not have access to a full graphical environment.

---

### Lecture 2.6: What Is Bash Scripting And What Are Some Advantages To Using It

# What Is Bash Scripting, and What Are Some Advantages to Using It?

In previous lessons, you learned about Bash and some of the common commands you might use. But Bash supports a full scripting language, which you can use to perform more complex automated tasks.

Bash scripting involves writing a sequence of Bash commands in a file, which you can then execute with Bash to run the contents of the file.

Let's look at what a bash script may look like:

```
#!/bin/bash

servers=("prod" "dev")

for server in "${servers[@]}"
do
  echo "Pulling $server"
  rsync --archive --verbose $server:/etc/nginx/conf.d/server.conf configs/$server.conf
done
```

This script pulls NGINX configuration files from a list of remote servers, which can be useful for backing up those configs into a local repository. NGINX is a popular web server and you will learn more about working with servers in a future module.

The first line is called a "shebang" (`#!`) and tells the system which interpreter should be used to run the script. Common values here are `/usr/bin/bash`, `/bin/bash`, or `/bin/sh`.

The first line, `servers=("prod" "dev")`, instantiates a list of strings representing the server names. `"prod"` is often used to refer to the production site, while `"dev"` refers to the development site, which is typically used for testing new features and changes before they are deployed to the live production environment.

Then, the list is iterated through with a `for` loop - the `servers[@]` syntax expands the list into individual elements. Each element is assigned to server with each iteration.

The `do` statement indicates the beginning of the loop's logical block, or the code that should run with each iteration.

`echo "Pulling $server"` interpolates the current value of the server variable, which would be prod or dev in this case, and logs it to the terminal.

Then `rsync` is used to pull the actual file from the server and save it locally, using more interpolation to manage that command.

`done` indicates the end of the loop's logical block.

There are a number of significant advantages to understanding and leveraging Bash scripting.

The first is that nearly every Unix environment comes with Bash readily available, which means you can run your script as-is without having to configure any language runtimes like Node.js or Python.

The second is that you have access to all of the binary applications available on the system with minimal effort. If your system has doctl installed, your script can execute that binary. A binary is a compiled program that the computer runs. When you have a bash script, you can execute the binary which will launch the program.

And finally, the syntax you use for your script is also executable directly in the terminal. This means that testing a small portion of your script becomes much less convoluted - you can copy and paste that portion directly into your terminal and see the result!

Understanding Bash will not only level up your scripting game, but will make you a wizard in the command line!

---

### Section Summary: Bash Commands

# Bash Commands Review

Terminal, Shell, and Command Line Basics
----------------------------------------

* **Command line**: A text interface where users type commands.
* **Terminal**: The application that provides access to the command line.
* **Terminal emulator**: Adds extra features to a terminal.
* **Shell**: Interprets the commands entered into the terminal (e.g., Bash).
* **PowerShell / Command Prompt / Microsoft Terminal**: Options for accessing the command line on Windows.
* **Terminal (macOS)**: Built-in option on macOS, with third-party alternatives like iTerm or Ghostty.
* **Terminal (Linux)**: Options vary by distribution, with many third-party emulators like kitty.
* **Terminology**: Though "terminal," "shell," and "command line" are often used interchangeably, they have specific meanings.

Command Line Shortcuts
----------------------

* **Up/Down arrows**: Cycle through previous/next commands in history.
* **Tab**: Autocomplete commands.
* **`Control+L`** (Linux/macOS) or typing `cls` (Windows): Clear the terminal screen.
* **`Control+C`**: Interrupt a running command (also used for copying in PowerShell if text is selected).
* **`Control+Z`** (Linux/macOS only): Suspend a task to the background; use `fg` to resume it.
* **`!!`**: Instantly rerun the last executed command.

Bash Basics
-----------

* **Bash** (Bourne Again Shell): Widely used Unix-like shell.  
  Key commands:

  + **`pwd`**: Show the current directory.
  + **`cd`**: Change directories.
    - **`..`** refers to the parent directory (one level up).
    - **`.`** refers to the current directory.
  + **`ls`**: List files and folders.
    - **`-a`**: Show all files, including hidden files.
    - **`-l`**: Show detailed information about files.
  + **`less`**: View file contents one page at a time with navigation options, including scrolling backward and searching.
  + **`more`**: Display file contents one screen at a time, with limited backward scrolling and basic navigation.
  + **`cat`**: Show the entire file content at once without scrolling or navigation, useful for smaller files.
  + **`mkdir`**: Create a new directory.
  + **`rmdir`**: Remove an empty directory.
  + **`touch`**: Create a new file.
  + **`mv`**: Move or rename files.
    - Rename: `mv oldname.txt newname.txt`
    - Move: `mv filename.txt /path/to/target/`
  + **`cp`**: Copy files.
    - **`-r`**: Recursively copy directories and their contents.
  + **`rm`**: Delete files.
    - **`-r`**: Recursively delete directories and their contents.
  + **`echo`**: Display a line of text or a variable's value.
    - Use `>` to overwrite the existing content in a file. (e.g., `echo "text" > file.txt`)
    - Use `>>` to append output to a file **without overwriting existing content** (e.g., `echo "text" >> file.txt`).
  + **`exit`**: Exit the terminal session.
  + **`clear`**: Clear the terminal screen.
  + **`find`**: Search for files and directories.
    - **`-name`**: Search for files by name pattern (e.g., `find . -name "*.txt"`).
  + Use **`man`** followed by a command (e.g., `man ls`) to access detailed manual/help pages.

Command Options and Flags
-------------------------

* **Options** or **flags**: modify a command's behavior and are usually prefixed with hyphens:
  + **Long form (two hyphens)**:
    - Example: `--help`, `--version`
    - Values are attached using an equals sign, e.g., `--width=50`.
  + **Short form (one hyphen)**:
    - Example: `-a`, `-l`
    - Values are passed with a space, e.g., `-w 50`.
    - Multiple short options can be chained together, e.g., `ls -alh`.
* **`--help`**: You can always use a command with this flag to understand the available options for any command.

---

### Section Summary: Bash Scripting

# Bash Scripting Review

Bash Scripting Basics
---------------------

* **Bash scripting**: Writing a sequence of Bash commands in a file, which you can then execute with Bash to run the contents of the file.
* **Shebang**: The commented line at the beginning of a script (e.g., `#!/bin/bash`) that indicates what interpreter should be used for the script.

  ```
  #!/bin/bash
  ```
* **Variable assignment**: Instantiate variables using the syntax `variable_name=value`.

  ```
  servers=("prod" "dev")
  ```
* **Variable creation rules**: Create variables with `VARIABLE_NAME=VALUE` syntax. No spaces are allowed around the equal sign (`=`). Use double quotes if the value contains spaces.

  ```
  NAME=John
  MESSAGE="Hello World"
  COUNT=5
  TEXT="The next number is, "
  ```
* **Variable usage**: Access variable values by placing `$` in front of the variable name.

  ```
  echo $NAME
  echo "The message is: $MESSAGE"
  ```
* **Variable interpolation**: Use `$variable_name` to access the value of a variable within strings and commands.

  ```
  TEXT="The next number is, "
  NUMBER=42
  echo $TEXT B:$NUMBER
  echo $TEXT I:$NUMBER

  echo "Pulling $server"
  rsync --archive --verbose $server:/etc/nginx/conf.d/server.conf configs/$server.conf
  ```
* **Variable scope**: Shell scripts run from top to bottom, so variables can only be used below where they are created.

  ```
  NAME="Alice"
  echo $NAME
  ```
* **User input**: Use `read` to accept input from users and store it in a variable.

  ```
  read USERNAME
  echo "Hello $USERNAME"
  ```
* **Comments**: Add comments to your scripts using `#` followed by your comment text.

  + Single-line comments start with `#` and continue to the end of the line
  + Comments are ignored by the shell and don't affect script execution

  ```
  # This is a single-line comment
  NAME="John"  # Comment at end of line
  ```
* **Multi-line comments**: Comment out blocks of code using colon and quotes.

  ```
  : '
  This is a multi-line comment
  Everything between the quotes is ignored
  Useful for debugging or documentation
  '
  ```
* **Built-in commands and help**:

  + Use `help` to see a list of built-in bash commands
  + Use `help <command>` to get information about specific built-in commands
  + Some commands (like `if`) are built-ins and don't have man pages
  + Built-in commands are executed directly by the shell rather than as external programs
  + Use `help function` to see information about creating functions

  ```
  help
  help if
  help function
  ```
* **Finding command locations**: Use `which` to locate where executables are installed.

  + Shows the full path to executable files
  + Useful for finding interpreter locations (like bash)
  + Helps verify which version of a command will be executed

  ```
  which bash
  which python
  which ls
  ```
* **Manual pages**: Use `man` to access detailed documentation for commands.

  + Provides comprehensive information about command usage
  + Shows all available options and examples
  + Use arrow keys to navigate, 'q' to quit
  + Not all commands have manual pages (built-ins use `help` instead)

  ```
  man echo
  man ls
  man bash
  ```
* **Help flags**: Many commands support `--help` for quick help information.

  + Alternative to manual pages for quick reference
  + Shows command syntax and common options
  + Not all commands support this flag (some may show error)

  ```
  ls --help
  chmod --help
  mv --help
  ```
* **Echo command options**: The `echo` command supports various options:

  + `-e` option enables interpretation of backslash escapes
  + `\n` creates a new line
  + Empty lines are only printed when values are enclosed in quotes
  + Useful for creating formatted output and program titles

  ```
  echo -e "Line 1\nLine 2"
  echo ""
  echo -e "\n~~ Program Title ~~\n"
  echo "Line 1\nLine 2"
  ```
* **Script arguments**: Programs can accept arguments that are accessible using `$` variables.

  + `$*` prints all arguments passed to the script
  + `$@` prints all arguments passed to the script as separate quoted strings
  + `$<number>` accesses specific arguments by position (e.g., `$1`, `$2`, `$3`)

  ```
  echo $*
  echo $@
  echo $1
  echo $2
  ```

Double Bracket Expressions `[[ ]]`
----------------------------------

* **Double bracket syntax**: Use `[[ ]]` for conditional testing and pattern matching.

  + Must have spaces inside the brackets and around operators
  + Returns exit status 0 (true) or 1 (false) based on the test result

  ```
  [[ $variable == "value" ]]
  [[ $number -gt 10 ]]
  [[ -f filename.txt ]]
  ```
* **String comparison operators**: Compare strings using various operators within `[[ ]]`.

  + `==` (equal): Tests if two strings are identical
  + `!=` (not equal): Tests if two strings are different
  + `<` (lexicographically less): String comparison in alphabetical order
  + `>` (lexicographically greater): String comparison in alphabetical order

  ```
  [[ "apple" == "apple" ]]
  [[ "apple" != "orange" ]]
  [[ "apple" < "banana" ]]
  [[ "zebra" > "apple" ]]
  ```
* **Numeric comparison operators**: Compare numbers using specific numeric operators.

  + `-eq` (equal): Numeric equality comparison
  + `-ne` (not equal): Numeric inequality comparison
  + `-lt` (less than): Numeric less than comparison
  + `-le` (less than or equal): Numeric less than or equal comparison
  + `-gt` (greater than): Numeric greater than comparison
  + `-ge` (greater than or equal): Numeric greater than or equal comparison

  ```
  [[ $number -eq 5 ]]
  [[ $count -ne 0 ]]
  [[ $age -ge 18 ]]
  [[ $score -lt 100 ]]
  ```
* **Logical operators**: Combine multiple conditions using logical operators.

  + `&&` (and): Both conditions must be true
  + `||` (or): At least one condition must be true
  + `!` (not): Negates the condition (makes true false, false true)

  ```
  [[ $age -ge 18 && $age -le 65 ]]
  [[ $name == "John" || $name == "Jane" ]]
  [[ ! -f missing_file.txt ]]
  ```
* **File test operators**: Test file properties and existence.

  + `-e file`: True if file exists
  + `-f file`: True if file exists and is a regular file
  + `-d file`: True if file exists and is a directory
  + `-r file`: True if file exists and is readable
  + `-w file`: True if file exists and is writable
  + `-x file`: True if file exists and is executable
  + `-s file`: True if file exists and has size greater than zero

  ```
  [[ -e /path/to/file ]]
  [[ -f script.sh ]]
  [[ -d /home/user ]]
  [[ -x program ]]
  ```
* **Pattern matching with `=~`**: Use regular expressions for advanced pattern matching.

  + `=~` operator enables regex pattern matching
  + Pattern should not be quoted when using regex metacharacters
  + Supports full regular expression syntax
  + Case-sensitive by default

  ```
  [[ "hello123" =~ [0-9]+ ]]
  [[ "email@domain.com" =~ ^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$ ]]
  [[ "filename.txt" =~ \.txt$ ]]
  ```
* **Variable existence testing**: Check if variables are set or empty.

  + Test if variable is empty: `[[ ! $variable ]]`

  ```
  [[ ! $undefined_var ]]
  ```

Double Parentheses Expressions `(( ))`
--------------------------------------

* **Arithmetic evaluation**: Use `(( ))` for mathematical calculations and numeric comparisons.

  + Evaluates arithmetic expressions using C-style syntax
  + Variables don't need `$` prefix inside double parentheses
  + Returns exit status 0 if result is non-zero, 1 if result is zero
  + Supports all standard arithmetic operators

  ```
  (( result = 10 + 5 ))
  (( count++ ))
  (( total += value ))
  ```
* **Arithmetic operators**: Mathematical operators available in `(( ))`.

  + `+` (addition): Add two numbers
  + `-` (subtraction): Subtract second number from first
  + `*` (multiplication): Multiply two numbers
  + `/` (division): Divide first number by second (integer division)
  + `%` (modulo): Remainder after division
  + `**` (exponentiation): Raise first number to power of second

  ```
  (( sum = a + b ))
  (( diff = x - y ))
  (( product = width * height ))
  (( remainder = num % 10 ))
  (( power = base ** exponent ))
  ```
* **Assignment operators**: Modify variables using arithmetic assignment operators.

  + `=` (assignment): Assign value to variable
  + `+=` (add and assign): Add value to variable
  + `-=` (subtract and assign): Subtract value from variable
  + `*=` (multiply and assign): Multiply variable by value
  + `/=` (divide and assign): Divide variable by value
  + `%=` (modulo and assign): Set variable to remainder

  ```
  (( counter = 0 ))
  (( counter += 5 ))
  (( total -= cost ))
  (( area *= 2 ))
  (( value /= 3 ))
  ```
* **Increment and decrement operators**: Modify variables by one.

  + `++variable` (pre-increment): Increment before use
  + `variable++` (post-increment): Increment after use
  + `--variable` (pre-decrement): Decrement before use
  + `variable--` (post-decrement): Decrement after use

  ```
  (( ++counter ))
  (( index++ ))
  (( --remaining ))
  (( attempts-- ))
  ```
* **Comparison operators**: Compare numbers using arithmetic comparison.

  + `==` (equal): Numbers are equal
  + `!=` (not equal): Numbers are not equal
  + `<` (less than): First number is less than second
  + `<=` (less than or equal): First number is less than or equal to second
  + `>` (greater than): First number is greater than second
  + `>=` (greater than or equal): First number is greater than or equal to second

  ```
  (( age >= 18 ))
  (( score < 100 ))
  (( count == 0 ))
  (( temperature > freezing ))
  ```
* **Logical operators**: Combine arithmetic conditions.

  + `&&` (and): Both conditions must be true
  + `||` (or): At least one condition must be true
  + `!` (not): Negates the condition

  ```
  (( age >= 18 && age <= 65 ))
  (( score >= 90 || extra_credit > 0 ))
  (( !(count == 0) ))
  ```
* **Bitwise operators**: Perform bit-level operations on integers.

  + `&` (bitwise AND): AND operation on each bit
  + `|` (bitwise OR): OR operation on each bit
  + `^` (bitwise XOR): XOR operation on each bit
  + `~` (bitwise NOT): Invert all bits
  + `<<` (left shift): Shift bits to the left
  + `>>` (right shift): Shift bits to the right

  ```
  (( result = a & b ))
  (( flags |= new_flag ))
  (( shifted = value << 2 ))
  ```
* **Conditional (ternary) operator**: Use `condition ? true_value : false_value` syntax.

  + Provides a concise way to assign values based on conditions
  + Similar to the ternary operator in C-style languages
  + Evaluates condition and returns one of two values

  ```
  (( result = (score >= 60) ? 1 : 0 ))
  (( max = (a > b) ? a : b ))
  (( sign = (num >= 0) ? 1 : -1 ))
  ```
* **Command substitution with arithmetic**: Use `$(( ))` to capture arithmetic results.

  + Returns the result of the arithmetic expression as a string
  + Can be used in assignments or command arguments
  + Useful for calculations that need to be used elsewhere

  ```
  result=$(( 10 + 5 ))
  echo "The answer is $(( a * b ))"
  array_index=$(( RANDOM % array_length ))
  ```

Control Flow and Conditionals
-----------------------------

* **Conditional statements**: Use `if` statements to execute code based on conditions.

  + Basic syntax: `if [[ CONDITION ]] then STATEMENTS fi`
  + Full syntax: `if [[ CONDITION ]] then STATEMENTS elif [[ CONDITION ]] then STATEMENTS else STATEMENTS fi`
  + Can use both `[[ ]]` and `(( ))` expressions for different types of conditions
  + **elif (else if)**: Optional, can be repeated multiple times to test additional conditions in sequence
  + **else**: Optional, executes when all previous conditions are false
  + Can mix double parentheses `(( ... ))` and double brackets `[[ ... ]]` in same conditional chain

  ```
  if (( NUMBER <= 15 ))
  then
      echo "B:$NUMBER"
  elif [[ $NUMBER -le 30 ]]
  then
      echo "I:$NUMBER"
  elif (( NUMBER < 46 ))
  then
      echo "N:$NUMBER"
  elif [[ $NUMBER -lt 61 ]]
  then
      echo "G:$NUMBER"
  else
      echo "O:$NUMBER"
  fi
  ```

Command Execution and Process Control
-------------------------------------

* **Command separation**: Use semicolon (`;`) to run multiple commands on a single line.

  + Commands execute sequentially from left to right
  + Each command's exit status can be checked individually

  ```
  [[ 4 -ge 5 ]]; echo $?
  ls -l; echo "Done"
  ```
* **Exit status**: Every command has an exit status that indicates success or failure.

  + Access exit status of the last command with `$?`
  + Exit status `0` means success (true/no errors)
  + Any non-zero exit status means failure (false/errors occurred)
  + Common error codes: `127` (command not found), `1` (general error)

  ```
  echo $?
  [[ 4 -le 5 ]]; echo $?
  ls; echo $?
  bad_command; echo $?
  ```
* **Subshells and command substitution**: Different uses of parentheses for execution contexts.

  + Single parentheses `( ... )` create a subshell
  + `$( ... )` performs command substitution
  + Subshells run in separate environments and don't affect parent shell variables

  ```
  ( cd /tmp; echo "Current dir: $(pwd)" )
  current_date=$(date)
  file_count=$(ls | wc -l)
  echo "Today is $current_date"
  echo "Found $file_count files"
  ```
* **Sleep command**: Pause script execution for a specified number of seconds.

  + Useful for creating delays in scripts
  + Can be used with decimal values for subsecond delays

  ```
  sleep 3
  sleep 0.5
  sleep 1
  ```

Loops
-----

* **While loops**: Execute code repeatedly while a condition is true.

  + Syntax: `while [[ CONDITION ]] do STATEMENTS done`

  ```
  I=5
  while [[ $I -ge 0 ]]
  do
      echo $I
      (( I-- ))
      sleep 1
  done
  ```
* **Until loops**: Execute code repeatedly until a condition becomes true.

  + Syntax: `until [[ CONDITION ]] do STATEMENTS done`

  ```
  until [[ $QUESTION =~ \?$ ]]
  do
      echo "Please enter a question ending with ?"
      read QUESTION
  done
  until [[ $QUESTION =~ \?$ ]]
  do
      GET_FORTUNE again
  done
  ```
* **For loops**: Iterate through arrays or lists using `for` loops with `do` and `done` to define the loop's logical block.

  ```
  for server in "${servers[@]}"
  do
      echo "Processing $server"
  done
  for (( i = 1; i <= 5; i++ ))
  do
      echo "Number: $i"
  done
  for (( i = 5; i >= 1; i-- ))
  do
      echo "Countdown: $i"
  done
  for i in {1..5}
  do
      echo "Count: $i"
  done
  ```

Arrays
------

* **Arrays**: Store multiple values in a single variable.

  + Create arrays with parentheses: `ARRAY=("value1" "value2" "value3")`
  + Access elements by index: `${ARRAY[0]}`, `${ARRAY[1]}`
  + Access all elements: `${ARRAY[@]}` or `${ARRAY[*]}`
  + Array indexing starts at 0

  ```
  RESPONSES=("Yes" "No" "Maybe" "Ask again later")
  echo ${RESPONSES[0]}     # Yes          
  echo ${RESPONSES[1]}     # No         
  echo ${RESPONSES[5]}     # Index 5 doesn't exist; empty string              
  echo ${RESPONSES[@]}     # Yes No Maybe Ask again later   
  echo ${RESPONSES[*]}     # Yes No Maybe Ask again later
  ```
* **Array inspection with declare**: Use `declare -p` to view array details.

  + Shows the array type with `-a` flag
  + Displays all array elements and their structure

  ```
  ARR=("a" "b" "c")
  declare -p ARR # ARR=([0]="a" [1]="b" [2]="c")
  ```
* **Array expansion**: Use `"${array_name[@]}"` syntax to expand an array into individual elements.

```
for server in "${servers[@]}"
```

Functions
---------

* **Functions**: Create reusable blocks of code.

  + Define with `FUNCTION_NAME() { STATEMENTS }`
  + Call by using the function name
  + Can accept arguments accessible as `$1`, `$2`, etc.

  ```
  GET_FORTUNE() {
      echo "Ask a question:"
      read QUESTION
  }
  GET_FORTUNE
  ```
* **Function arguments**: Functions can accept arguments just like scripts.

  + Arguments are passed when calling the function
  + Access arguments inside function using `$1`, `$2`, etc.
  + Use conditional logic to handle different arguments

  ```
  GET_FORTUNE() {
      if [[ ! $1 ]]
      then
          echo "Ask a yes or no question:"
      else
          echo "Try again. Make sure it ends with a question mark:"
      fi
      read QUESTION
  }
  GET_FORTUNE
  GET_FORTUNE again
  ```

Random Numbers and Mathematical Operations
------------------------------------------

* **Random numbers**: Generate random values using the `$RANDOM` variable.

  + `$RANDOM` generates numbers between 0 and 32767
  + Use modulo operator to limit range: `$RANDOM % 75`
  + Add 1 to avoid zero: `$(( RANDOM % 75 + 1 ))`
  + Must use `$(( ... ))` syntax for calculations with `$RANDOM`

  ```
  NUMBER=$(( RANDOM % 6 ))
  DICE=$(( RANDOM % 6 + 1 ))
  BINGO=$(( RANDOM % 75 + 1 ))
  echo $(( RANDOM % 10 ))
  ```
* **Random array access**: Use random numbers to access array elements randomly.

  + Generate random index within array bounds
  + Use random index to access array elements
  + Useful for random selections from predefined options

  ```
  RESPONSES=("Yes" "No" "Maybe" "Outlook good" "Don't count on it" "Ask again later")
  N=$(( RANDOM % 6 ))
  echo ${RESPONSES[$N]}
  ```
* **Modulo operator**: Use `%` to get the remainder of division operations.

  + Essential for limiting random number ranges
  + Works with `$RANDOM` to create bounded random values
  + `RANDOM % n` gives numbers from 0 to n-1

  ```
  echo $(( 15 % 4 ))
  echo $(( RANDOM % 100 ))
  echo $(( RANDOM % 10 + 1 ))
  ```

Environment and System Information
----------------------------------

* **Environment variables**: Predefined variables available in the shell environment.

  + `$RANDOM`: Generates random numbers between 0 and 32767
  + `$LANG`: System language setting
  + `$HOME`: User's home directory path
  + `$PATH`: Directories searched for executable commands
  + View all with `printenv` or `declare -p`

  ```
  echo $RANDOM
  echo $HOME
  echo $LANG
  printenv
  ```
* **Variable inspection**: Use `declare` to view and work with variables.

  + `declare -p`: Print all variables and their values
  + `declare -p VARIABLE`: Print specific variable details
  + Shows variable type (string, array, etc.) and attributes

  ```
  declare -p
  declare -p RANDOM
  declare -p MY_ARRAY
  ```
* **Command types**: Different categories of commands available in bash.

  + **Built-in commands**: Executed directly by the shell (e.g., `echo`, `read`, `if`)
  + **External commands**: Binary files in system directories (e.g., `ls`, `sleep`, `bash`)
  + **Shell keywords**: Language constructs (e.g., `then`, `do`, `done`)
  + Use `type <command>` to see what type a command is

  ```
  type echo
  type ls
  type if
  type ./script.sh
  ```

File Creation and Management
----------------------------

* **File creation**: Use `touch` to create new empty files.

  + Creates a new file if it doesn't exist
  + Updates the timestamp if the file already exists
  + Commonly used to create script files before editing

  ```
  touch script.sh
  touch bingo.sh
  touch filename.txt
  ```

Creating and Running Bash Scripts
---------------------------------

* **Script execution methods**: Multiple ways to run bash scripts:
  + **`sh scriptname.sh`**: Run with the sh shell interpreter.
  + **`bash scriptname.sh`**: Run with the bash shell interpreter.
  + **`./scriptname.sh`**: Execute directly (requires executable permissions).

```
sh questionnaire.sh
bash questionnaire.sh
./questionnaire.sh
```

File Permissions and Script Execution
-------------------------------------

* **Permission denied error**: When using `./scriptname.sh`, you may get "permission denied" if the file lacks executable permissions.
* **Checking permissions**: Use `ls -l` to view file permissions.

  ```
  ls -l questionnaire.sh
  ```
* **Permission format**: The output shows permissions as `-rw-r--r--` where:

  + First character (`-`): File type (- for regular file, d for directory)
  + Next 9 characters: Permissions for owner, group, and others
  + `r` = read, `w` = write, `x` = execute
* **Adding executable permissions**: Use `chmod +x` to give executable permissions to everyone.

  ```
  chmod +x questionnaire.sh
  ```
* **Script organization**: Best practices for structuring bash scripts.

  + Start with shebang (`#!/bin/bash`)
  + Add descriptive comments about script purpose
  + Define variables at the top
  + Group related functions together
  + Main script logic at the bottom

  ```
  #!/bin/bash
  NAME="value"
  ARRAY=("item1" "item2")
  my_function() {
      echo "Function code here"
  }
  my_function
  echo "Script complete"
  ```
* **Sequential script execution**: Create master scripts that run multiple programs in sequence.

  + Useful for automating workflows that involve multiple scripts
  + Each script runs to completion before the next one starts
  + Can combine different programs into a single execution flow
  + Arguments can be passed to individual scripts as needed
  + Can include different types of programs (interactive, automated, etc.)

  ```
  #!/bin/bash
  ./setup.sh
  ./interactive.sh
  ./processing.sh
  ./cleanup.sh
  ```

---

## Module 3: Version Control Fundamentals (Git & GitHub Basics)

### Lecture 3.1: What Is Version Control And Why Are These Systems Necessary

# What Is Version Control, and Why Are These Systems Necessary?

If you've worked on something, like a thesis paper, where you've saved copies after making significant changes and named the files something like `Thesis-Draft`, `Thesis-Final`, `Thesis-Final-For-Real`, and `Thesis-Absolute-Final-DO-NOT-CHANGE`, you've used a very rudimentary approach to version control. But what if I told you there is a better way?

You may have heard of tools like Git, SVN, or Mercurial before. These are version control systems, and they are a key component to every developer's workflow. A version control system allows you to track and manage changes in your project. For the purposes of these lessons, we will be focusing on Git.

Git offers powerful tools that allow you to manage the edit history of a project. You will learn more about how to use Git and the features it offers in upcoming lessons. For now, here's what you really need to know:

Git allows you to do things like create commits, which are a snapshot of a specific state of your codebase. You can then compare commits to see what changes you have made, revert a commit that has improper changes, and more.

You can also create "branches", which you can think of as different pathways in your code. While a branch might be the road you walk down, commits are the landmarks along the way. Branches allow you to do things like work on a new feature in isolation, such that if your work goes sideways you can delete the branch without impacting the core codebase.

These features make version control an essential component of collaboration with other developers. When you have multiple people working in the same project, branches allow each of them to work on their own code without running over each other's changes.

You will often pair a version control system like Git with a version control provider like GitHub or Gitlab, which offers you additional collaboration tools and the ability to back up your projects to the cloud.

But even without a cloud-based storage solution, version control systems can be a game changer for your workflows. No more `THIS-IS-THE-FINAL-COPY-FOREVER` files.

There's a lot of cool information to cover about using these systems, so let's do a deep dive in the next few lessons!

---

### Lecture 3.2: What Is The Purpose Of Sites Like Github And Gitlab

# What Is the Purpose of Sites Like GitHub and GitLab, and What Are Some Benefits of Using Them?

In a previous lesson, we briefly mentioned GitHub. Both GitHub and Gitlab are version control providers. This means they are cloud-based solutions that offer storage of version-controlled projects in something called "repositories", and enable collaboration features to use with those projects.

Before we dive in to the features these platforms offer, we need to discuss the different types of projects. Many projects are considered "open-source", which means people can see the code you publish, propose changes, report issues, and even run a modified version.

But sometimes you may only want your teammates to see and work on the code. You can also publish a project as "closed-source", meaning the only people who can see and interact with the project are the people you explicitly authorize.

Regardless of which approach your project takes, sites like GitHub and Gitlab can massively level up your team's collaboration.

For example, a teammate working on a feature might be stuck and have questions. Rather than having to copy-paste the code into Discord for you to read, or hop on a call to screen share their work, they can upload the changes directly to GitHub. From there, you can view the changes in your browser or even download the changes to run and debug locally.

When a teammate has completed a feature, they can propose the changes through these websites. You are then able to review the changes, leaving comments on specific files or lines if you have thoughts and questions. You can even propose suggested edits which they can apply to the changes right there in the browser!

If you are happy with the changes, you can accept them and merge them into your primary branch. This means the entire team can then download the latest changes locally so they have the most up-to-date code when they start on their next task.

Speaking of tasks, these sites also offer powerful issue trackers. You can use these to track and assign tickets to your team members, accept bug reports from the public, and even plan full sprints through things like the project boards.

There are many more features offered by these sites. In the next few lessons, we'll cover the key aspects so you can dive right in and start collaborating!

---

### Lecture 3.3: How Do You Install And Set Up Git

# How Do You Install and Set Up Git?

Before you can really start to make use of version control, and sites like GitHub, you need to have Git installed and ready to use.

To check if Git is already installed on your machine you can run the following command in the terminal:

```
git --version
```

If you see a version number, that means Git is installed. If not, then you will need to install it.

For Linux systems, Git often comes preinstalled with most distros. If you do not have Git pre-installed, you should be able to install it with your package manager commands such as `sudo apt-get install git` or `sudo pacman -S git`.

For Mac users, you can install Git via Homebrew with `brew install git`, or you can download the executable installer from Git's website.

For Windows, you can download the executable installer from Git's website. Or, if you have set up Chocolatey, you can run `choco install git.install` in PowerShell. Note that on Windows, you may also want to download GitBash so you have a Unix-like shell environment available.

To make sure the installation worked, run the `git --version` command again in the terminal.

Once you have Git installed, you will need to make a few changes to the configuration. You should only need to make these changes once on your computer and you won't need to continually make changes when you make upgrades.

`git config` is used to set configuration variables that are responsible for how Git operates on your machine. To view your current setting variables and where they are stored on your system, you can run the following command:

```
git config --list --show-origin
```

Right now you should be seeing only system-level configuration settings if you just installed Git for the first time. If you have already installed Git prior to this lesson, then you might be seeing user configurations for a user name and email.

To set your user name, you can run the following command:

```
git config --global user.name "Jane Doe"
```

The `--global` flag is used here to set the user name for all projects on your system that use Git. If you need to override the user name for a particular project, then you can run the command in that particular project directory without the `--global` flag.

To set the user email address, you can run the following command:

```
git config --global user.email janedoe@example.com
```

Configuring your user name and email is important because Git will use this information for every commit you make in a project. You will learn more about commits in a future lesson.

Another configuration you can set is the preferred editor you want Git to use. Here is an example of how to set your preferred editor to Emacs:

```
git config --global core.editor emacs
```

Other options include Vim, Nano, VS Code, and more. For example, if you use VS Code for your editor, then you can configure Git settings like this:

```
git config --global core.editor "code --wait"
```

If you choose not to set a preferred editor, then Git will default to your system's default editor.

If you are using a Windows machine and want to change your editor, you will need to provide the complete path to the executable file like this:

```
git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"
```

To see your list of configurations, you can run the following command:

```
git config --list
```

Now that you have Git installed and set up, you are now ready to start adding version control to your projects.

---

### Lecture 3.4: How Do You Handle Security Requirements Like Ssh And Gpg Keys

# How Do You Handle Security Requirements Like SSH and GPG Keys?

Before you can push your repository to GitHub, you will need to be authenticated. Both SSH and GPG keys use a public-private pair. This means that you keep a private key on your local machine, which you use to authenticate yourself. You share a public key with the people or services that need to validate your auth. In other words, the private key is required to perform an action, and the public key is used to verify the action.

GPG, or Gnu Privacy Guard, keys are typically used to sign files or commits. Someone can then use your public GPG key to verify that the file signature is from your key and that the contents of the file have not been modified or tampered with. SSH, or Secure SHell, keys are typically used to authenticate a remote connection to a server - via the `ssh` utility. However, as you'll learn in this lesson, you can also use an SSH key to sign commits.

To generate a GPG key, you'll need to run:

```
gpg --full-generate-key
```

For an SSH key, you'll run:

```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Make sure to provide your actual email.

Both of these commands should request a passphrase to secure the key. These are optional, but strongly recommended.

For SSH keys, you'll get two files - one for your private key, and one for your public. Public key filenames will end in `.pub`, so you do not accidentally share your private key. These files will be in `~/.ssh`.

GPG keys, however, will be in a hidden and encrypted directory. Instead, to list your public keys, you'll run:

```
gpg --list-secret-keys --keyid-format=long
```

Then, to get the public key, use:

```
gpg --armor --export "<key id>"
```

But what can you do with these new keys? Well, we've talked about signing your commits, and that's something you can use either of these keys for.

In order to sign your commits with your GPG key, you'll need to upload your public key, not the private key, to your GitHub account. Then, take the short ID you got from listing the keys earlier, and run this command to set it as your git signing key:

```
git config --global user.signingkey <your_gpg_key_id>
```

Then, you can pass the `-S` flag to your `git commit` command to sign a specific commit - you'll need to provide your passphrase. Alternatively, if you want to sign every commit automatically, you can set the autosign config to `true`:

```
git config --global commit.gpgsign true
```

To sign with an SSH key, which is a relatively new feature on GitHub, you'll need to start by uploading the key to your GitHub account. Then you'll need to set the signing mode for git to use SSH:

```
git config --global gpg.format ssh
```

Then, to set the signing key, you'll pass the file path instead of an ID:

```
git config --global user.signingkey <path_to_your_ssh_keys>
```

Finally, you can enable auto signing as you would for a GPG key.

With either of these approaches set up, you're now set to have verified commits which will get a special badge on GitHub.

---

### Lecture 3.5: What Is A Repository And How Do You Create One

# What Is a Repository, and How Do You Create One?

We've talked a bit about Git and GitHub, so now we can start to put it all together. In order to do this, you need a repository. But what is a repository? You can think of a repository as a container for a project - if you are working on an app, you would keep the files for that app together in a repository.

Repositories can be local on your computer, or remote on a service like GitHub. To create a repository, you can start with either local or remote - the result will be the same, so take whatever approach fits your workflow best. For a workflow where you start with a remote repository, you can create one directly through GitHub's website by following these instructions:

Visit [GitHub's website](https://github.com), make sure you are logged in, and then click the plus icon in the top right of the navigation bar. You'll see quite a few options, but the one you care about is "New Repository". Select that to open the UI for creating a new repository.

The first option you'll see there is the ability to choose a template. You likely do not have one of these set up yet, but a template is a special kind of repository that you can use as a springboard for your new repositories. These are helpful for including documentation or issue templates in all of your projects.

Your next option is to select an owner, you can choose your user account or any organizations you own or have access to. Then you can name the repository - in general, you'll want to use a name that succinctly describes the project you are building. As a general best practice, you want to avoid spaces in your repo name. GitHub will automatically replace them with hyphens.

Next, you can optionally add a description which will appear on the repository's home page.

You can also choose whether the repository will be public or private. A public repository can be viewed and downloaded by anyone. A private repository can only be accessed by you, and anyone you grant explicit access to.

Finally, if you do not select a template, you will see options to generate files in the repository automatically. A README file will appear on the repository's homepage, and is a great way to provide documentation and descriptions of your project. A `.gitignore` file allows you to specify files that Git will "ignore" - this is great for things like package dependencies, environment files, and other things you don't want to be saved. GitHub will offer templates for this file, which exclude the common items for the specified language or runtime. And a license is a legal document which outlines who may use your software, and what they may do with it.

When you have your settings all configured as you like, you can click the "Create Repository" button to finish the process. You'll automatically be redirected to the landing page for your new repository!

From here, you can click the "Code" button to get options to clone your repository to your computer.

You can ignore the "Codespaces" and "Copilot" tabs for this lesson. Instead, we are going to focus on the three options in the "Local" tab. The first two, HTTPS and SSH, are used in the same way. You use the `git clone` command with the URL provided in the box to clone the remote repository to your computer. The difference between these two is the connection and authentication methods.

For cloning a public repository, you won't actually need to authenticate. But to clone a private repository, or to push to either public or private repositories, you will have to be authenticated. An HTTPS remote URL used to authenticate you via your GitHub username and password. However, due to security concerns this is no longer supported, and you are instead required to use a username and access token. Even then, it's a much less secure method than SSH, which uses your private and public keys. This has an added benefit of automatically signing you in, rather than having to provide a token every time. There will be a separate lesson diving deeper into SSH and how it works but you can also read through the GitHub documentation on how to setup SSH.

To clone the repository, you can run this in the terminal:

```
git clone git@github.com:your-username/your-repository-name
```

It will create a folder on your computer with your repository name and contain all the files from your repository within it. From there you can `cd` (change directory) to your cloned repository with:

```
cd name-of-cloned-repo
```

Additionally, the local copy of your repo will have a remote pointing to the copy on GitHub. To check your remotes you can run the following command:

```
git remote -v
```

Another option for cloning your repository is to use the GitHub CLI. This tool is used to do GitHub-specific tasks without leaving the command line. If you do not have it installed, you can get instructions to do so from GitHub's documentation - but you should have it available in your system's package manager.

To clone a repository with the CLI tool, I would use:

```
gh repo clone your-username/your-repository-name
```

The end result of these commands is the same: you'll have a copy of your repository locally.

You can also use the GitHub CLI to create a repository:

```
gh repo create
```

If you don't pass any arguments, the CLI will give you an interactive wizard to set up your repository. This wizard will give you all of the same options as the web UI. With this tool, you will also get the option to clone the new repository immediately, so you won't have to go through the manual steps outlined earlier.

You now have a basic understanding of how repositories work, and how you can create one to start properly versioning your work. In future lessons, you will learn how to push an existing local repository to GitHub and how to push changes to remote repositories.

---

### Lecture 3.6: How Do You Push A Local Repository To Github

# How Do You Push a Local Repository to GitHub?

In a previous lesson, you learned how to create a new repository on GitHub. But what if you had an existing project locally that you want to add to GitHub? In this lesson, you will learn how to push existing local repositories to GitHub and pull changes down from remote repositories.

Start by creating a new repository on GitHub without any files. When done correctly, you should be redirected a page that includes the URL needed to clone your repository.

Now navigate to your terminal and select an existing project you wish to add to GitHub. In this lesson, I am choosing a local project called `super-awesome-game` with the following files inside:

```
jessicawilkins super-awesome-game >> ls
README.md  index.html script.js  styles.css
```

To setup version control for this project using Git, you will need to run the `git init` command in the project directory. This will initialize an empty Git repository so Git can begin tracking changes for this project. When done correctly you should see a similar output in the terminal:

```
jessicawilkins super-awesome-game >> git init
Initialized empty Git repository in /Users/jessicawilkins/workspace/freeCodeCamp/super-awesome-game/.git/
```

When you initialize an empty Git repository to a project, a new `.git` hidden directory will be added. To view the addition of the directory you can run the `ls -a` command which lists all files and directories, including hidden ones:

```
jessicawilkins super-awesome-game >> ls -a
.          ..         .git       README.md  index.html script.js  styles.css
```

It is important not to delete that `.git` directory, otherwise all of your Git history will be lost.

Now that the empty Git repository has been initialized, you can run the `git status` command. This command is used to show the current state of your working directory - you will be using this command a lot in your workflow. You should see an output similar to this:

```
jessicawilkins super-awesome-game >> git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	README.md
	index.html
	script.js
	styles.css

nothing added to commit but untracked files present (use "git add" to track)
```

`On branch main` means that you are on the `main` branch. A branch in Git is a separate workspace where you can make changes. The `main` branch will often represent the primary or production branch in a real world application. Developer teams will create multiple branches for new features and bug fixes and then merge those changes back into the `main` branch. You will learn more about that process in a future lesson.

`Untracked files` means that Git has detected files that it is currently not tracking.

There are five states that a file can be in:

1. "Untracked": This means that the file is new to the repository, and Git has not "seen" it before.
2. "Modified": This file existed in the previous commit, and has changes that have not been committed.
3. "Ignored": You likely won't see ignored files in Git, but your IDE might have an indicator for them. Ignored files are excluded from Git operations, typically because they are included in the `.gitignore` file.
4. "Deleted": A deleted file is the opposite of an untracked file - it's a file that previously existed, and has been removed.
5. "Renamed": A renamed file is a file where the contents are unchanged, but the name or location of the file was modified. In some cases, a file can be considered renamed even if it has a small amount of changes.

When you have uncommitted changes in your repo, you will need to first "stage" them. A "staging area" is a special file in your `.git` directory that contains information that will go into your next commit. A commit is effectively a snapshot of the current state of your repository.

If you want to stage one file at a time, then you can use the following command:

```
git add name-of-file
```

If you want to stage all unstaged changes, then you can use `git add .` The period (`.`) is an alias for the current directory you are in. Some developers will warn against using `git add .` because you might end up staging files that you didn't intend to. If that happens, you can "unstage" them using the following command:

```
git reset name-of-file
```

In general though, as long as you are monitoring which files are being added using `git status` before you stage them, you should be fine.

Once you stage your files, then you will need to commit them. You can commit your changes by running the `git commit` command. This will open up your preferred editor of choice you set in the Git configuration. Once the editor is open, you can provide a detailed message of your changes. You can also choose to provide a shorter message by using the `git commit -m` command like this:

```
git commit -m "short message goes here"
```

If you are going to use the `-m` flag, you will still want to provide a descriptive message to provide context for the changes. Here are some examples of good messages you might use:

```
git commit -m "feat(api): implement JWT-based authentication"
git commit -m "fix(auth): correct token expiration time"
git commit -m "refactor: simplify login flow logic"
```

The `feat(api)` and `fix(auth)` follows the Conventional Commits style which is used to provide context on the types of changes in that commit.

After you have committed your work, and run `git status` again, you should see the following output in the terminal:

```
On branch main
nothing to commit, working tree clean
```

To view all of your prior commits for this project you can run the `git log` command. This will list all prior commits with helpful information like the author, date of commit, commit message and commit hash. The commit hash is a long string which serves as a unique identifier for a commit.

Once you are done committing your work, you can now push your changes to GitHub. You will first need to setup the remote connection to your remote repo. You learned about this in the previous lesson, but here is a reminder using SSH:

```
git remote add origin git@github.com:your-github-username/name-of-repo.git
```

The last step is to push your changes to GitHub using this command:

```
git push -u origin main
```

The `-u` flag is shorthand for `--set-upstream`. It connects your local `main` branch to the remote `main` branch on `origin`. You only need to use it once per new branch. After that, you can simply run `git push` without specifying the branch name.

When done correctly, you should see a similar result in the terminal:

```
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 253 bytes | 253.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/jdwilkin4/super-awesome-game.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
```

You should also see the new changes on your GitHub repo page when you refresh the page.

If you are collaborating with others on a project and need to pull down new changes from the repository, you can use the `git pull` command. You will learn more about working on a team and collaboration in a future lesson.

---

### Lecture 3.7: How Do You Create A New Branch For Your Repository

# How Do You Create a New Branch for Your Repository?

You've previously learned how to commit changes and push them up to your remote repository, but all of that has been on your default `main` branch. That can work for a smaller project, but as you contribute to other open source projects, or as your project grows, branches are essential.

For example, if you fork a repository and make commits to the `main` branch of your fork, you may end up with changes in your fork that the original repository did not accept. This can make it incredibly difficult to update your branch with the changes from the fork that were accepted. Or, when working on your own project, switching between different tasks becomes much more difficult if you are not using branches. Instead, you have to manually keep track of which changes relate to which feature or fix.

But what exactly is a branch? Consider your `main` branch as a highway, with each commit being a car that enters the highway. You may decide you want to go take a look at something, like creating a new feature, so you need to get off of the highway for a bit to go see.

A branch is essentially a deviation from your main history, where you can freely play around with changes for a new feature or a bug fix. If you are happy with your changes, you can get back on the highway by merging the branch into `main`. If you aren't happy with your changes, you can delete the branch and switch back to `main` without accepting the changes.

Before creating a new branch, you view your branches with the `git branch` command. The output might look like this:

```
* main
```

Right now we only have the one branch, our default `main` branch. The asterisk (`*`) means that is the branch that you currently have "checked out". You'll learn more about that in a bit.

You can create a new branch with the `git branch` command, with an argument to specify the new branch's name:

```
git branch feature
```

This creates a new branch named `feature`. Let's take a look at our branches again with `git branch`:

```
  feature
* main
```

We can now see our new branch, but we are still on the `main` branch. We need to switch to our new branch by "checking it out". When you check out a new branch, you're telling Git to load the files in the exact state they were in at that point.

Let's check out our new branch with:

```
git checkout feature
```

or

```
git switch feature
```

And run `git branch` again to see:

```
* feature
  main
```

Notice that the asterisk has now moved to the branch you currently have "checked out".

Often times when you create a new branch, you will want to check it out immediately. Instead of creating the branch and then checking it out using two commands, you can create and switch to a branch in one command with:

```
git checkout -b feature
```

or

```
git switch -c feature
```

So now we've created and checked out a new branch. This branch is a clone of the `main` branch, it has all the same code that `main` did at the time you created the branch. Now, we can add any code to this branch without affecting the `main` branch. We've essentially gotten off the highway to create a feature. If you check your `git status`, you would see something like this:

```
On branch feature
nothing to commit, working tree clean
```

Create a new `feature.md` file by running this:

```
echo "This is our new feature" > feature.md
```

And now the status will look like this:

```
On branch feature
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	feature.md

nothing added to commit but untracked files present (use "git add" to track)
```

Next, it's time to commit your new feature. First, add the file to staging:

```
git add feature.md
```

Then, commit the changes:

```
git commit -m "my new feature"
```

Finally, push your `feature` branch to your repository:

```
git push -u origin feature
```

The `-u` flag connects your local `feature` branch to the remote one, so future pushes can be done with just `git push`.

Next, we will learn how to make a pull request for our new feature!

---

### Lecture 3.8: What Is A Pull Request And How Do You Create One

# What Is a Pull Request, and How Do You Create One?

In the previous lesson, we created a feature branch, committed a new file to that branch, and pushed it up to our remote repository. But what are our next steps? We need to create a pull request on GitHub.

A pull request is, effectively, a request to pull changes in from your branch into the target branch. Pull requests are the flow you use when you want to contribute code changes to an open source project. This approach allows the maintainers of the project to review your changes. They can leave comments, ask questions, suggest tweaks, and (hopefully) approve your changes and merge them in!

Let's head over to our repository on GitHub again.

Now, after you pushed your new branch, you should see a fancy banner that says you've pushed to a branch, and a button you can click to create a pull request. This button skips a couple of steps and streamlines the process, so we're going to ignore it for now. That way you are prepared for cases where the banner does not appear.

Click on the pull requests tab at the top the repository page, then ignore the banner again and click "New Pull Request". You'll be taken to a UI to prepare your request.

Now, there are some terms we need to go over here. First, we have the "base" and "compare" drop downs. The "base" is your target for the merge. Since we want to merge into `main`, we can leave this alone.

The "compare" is what you want to merge. We want to merge our `feature` branch, so we should change this to `feature`. This is also known as the head branch, which is a term you will want to remember.

Once you do this, the UI will refresh. It should now show the commits on `feature` that are not on `main`, indicating what you are requesting to merge in. You'll also see what's called a "diff", which is a visual representation of the actual changes you've made.

Because all we've done is add a file, the diff is pretty clean. For more complex changes, GitHub will highlight things like line modifications, additions, deletions, and more. Understanding how to read a diff can be challenging, but with some practice you will become quite proficient at it.

For now, let's go back to our pull request. There is a small link at the top that reads "compare across forks". If we were working from our fork of the freeCodeCamp repository, this would give us the ability to change our PR to target the original freeCodeCamp repo, instead of just the `main` branch within our fork.

Since we are not working with a fork, we can ignore this. However, it is very important to understand that what we are doing here is primarily for learning and exploration. You shouldn't open a PR to someone's project that just contains practice changes - this creates extra noise for the maintainers.

Now, since we are happy with our changes and everything is configured, we can click the "Create Pull Request" button. This takes us to a new UI.

Toward the bottom and out of view are the same commit list and diff view we saw earlier. It never hurts to double check one last time before creating your PR, but for this exploration you are good to move forward.

You'll also see a couple of new inputs. The first input is the title for your pull request. GitHub will automatically generate this based on the commit you are merging, if there is only one in the PR, or the branch name, if you have multiple commits.

The second input is for your description. In most cases, this will not be empty. Instead, maintainers of a project can define a template which gets pre-populated. If they provide one, you should respect their workflow and complete the template.

In both cases, you'll want to read the contributing documentation for the project to ensure you understand and follow their guidelines for how to title and fill out your PR.

Since you own this repository, you'll see on the right that you can set reviewers, assignees, labels, projects, and milestones. You won't be able to edit these, except to request a review, when you contribute to someone else's project. But if you'd like to explore those features, you can set them however you like now since this is your repository.

Once everything is filled out and configured, click "Create pull request". Finally, you'll see the actual result!

When you make a pull request to someone else's project, it needs to go through a "code review". This is a process where the maintainers can evaluate your pull request, request changes, ask questions, and so on. Once the maintainers have approved it, they can merge it.

Since this is your own project, you don't need to wait for a review. Instead, you can double check the commit history under the Commits tab, the changes under the Files changed, and if you are satisfied you can merge it.

After it's merged, you will want to pull these changes to your local repo.

Head back to your terminal, and make sure you are still in the repo's folder. Then switch to the `main` branch with `git checkout main`.

Next, pull down the latest changes with `git pull`.

Now, if you look at the commit history with `git log`, you will see your commit. But you will also see a `Merge pull request #1` message. What is that?

Well, when you merge a pull request on GitHub there are three strategies you can use:

The default is "Merge", which brings all of the commits from the head branch, then creates another commit to process and log the merge.

Another option is "Squash and Merge", which takes ALL of the commits from the head branch, smashes them into a single commit, and merges that new commit directly into the base branch without creating a merge commit.

Finally, there is "Rebase and Merge", which takes all of the commits, resets them to "come after" the latest commit on the base branch, then merges the head in without a merge commit. Rebasing is a complicated topic that you will learn about in depth later, so it's okay if you do not quite understand it today.

Each open source project will choose whatever merge strategy works best. But because of these differences in behavior, you should ALWAYS create a new branch to commit your contributions on. Never commit directly to the default `main` branch, or things will get messy when you need to bring the changes down from the original repo.

With all of that, you have successfully created and merged your first pull request!

---

### Lecture 3.9: How Do You Contribute To Other Peoples Repositories

# How Do You Contribute to Other People's Repositories?

You've learned about creating commits and pushing them up to your own repository that you control. You can do the same for other projects that you do not maintain, but there are some extra steps.

First and foremost, you generally won't have "write access" to someone else's project. This means you cannot push commits directly to them. Instead, you'll need to create a copy of the repository to work from. This process is called "forking".

To fork a repository, visit the repository you want to contribute to on GitHub. At the top, you'll see a "Fork" button. Click this to be taken to the UI for creating your fork.

You'll see a similar screen to the one where you created your own repository, but with fewer options. You can choose an owner, either your personal account or an organization you have access to, a new name for the fork, and a new description.

You also have an option to copy only the `main` branch (or the default configured for the repository). This is generally a good idea, unless you need to contribute to a specific feature branch. You'll learn more about branches in a future lesson. For now, leave that box ticked.

Click "Create fork" and your new repository will be created, and you'll automatically be taken to it.

Next, clone it to your local computer just like you would do with your own repository, using SSH or the GitHub CLI.

Now, let's take a look at the remotes your local clone has configured. Open a terminal in the local repository directory and run `git remote -v` to get a full list, it should look something like this:

```
origin git@github.com:your-username/your-repo-name.git (fetch)
origin git@github.com:your-username/your-repo-name.git (pull)
```

By cloning a repository from GitHub, Git has automatically configured your fork as the `origin` remote. However, when you're working from a fork, you will often need to update your copy to bring in the changes from the original repository.

To do this, let's add the original repository as another remote. Return to the page where you forked the repository from, click the "Code" button, and grab the SSH URL. Then run the command to create a new upstream remote:

```
git remote add upstream git@github.com:original-repo-username/repo-name.git
```

`upstream` is the name of the remote - you can name it something else, but `upstream` tends to be the convention. If you look at your remotes again, you will see your new upstream remote:

```
origin git@github.com:your-username/your-repo-name.git (fetch)
origin git@github.com:your-username/your-repo-name.git (pull)
upstream git@github.com:original-repo-username/your-repo-name.git (fetch)
upstream git@github.com:original-repo-username/your-repo-name.git (pull)
```

With the `upstream` remote you'll be able to do things like `git fetch upstream` and `git merge upstream/main` to get the latest changes from the original project into your local fork.

A fork is still a repository, and you create commits and push changes in the same way. However, before diving into that, you should understand that there are certain strategies that you should follow when making changes to someone else's project. You'll learn more about these strategies in upcoming lessons.

Projects which make their source code available to the public, allow you to modify the code, and accept code contributions are called "open source" projects. There are a lot of benefits to open source, such as allowing the community to help you identify and fix bugs, learning from the contributions people make to your work, and fostering a community of developers that you can turn in to a network.

When you make changes to someone's project, you are considered an "open source contributor". Contributing to open source projects can be an excellent preview of what working on a professional developer team is like. And some of the strategies here will help you do just that, and carry over into your first paid role.

And if you ever have questions about how to contribute, most open source projects will have contributing guidelines that contain an overview of everything you need to know. But if you still aren't sure, it never hurts to open an issue on the repository to ask your questions - or, if they have a community space on a platform like Discord, join and ask your questions there.

---

### Section Summary: Git

# Git Review

Introduction to Version Control
-------------------------------

* **Definition**: A version control system allows you to track and manage changes in your project. Examples of version control systems used in software are Git, SVN, or Mercurial.

Cloud-Based Version Control Providers
-------------------------------------

* **List of Cloud-Based Version Control Providers**: GitHub and GitLab are popular examples of cloud-based version control providers that allow software teams to collaborate and manage repositories.

Installing and Setting up Git
-----------------------------

* **Installing Git**: To check if Git is already installed on your machine you can run the following command in the terminal:

```
git --version
```

If you see a version number, that means Git is installed. If not, then you will need to install it.

For Linux systems, Git often comes preinstalled with most distros. If you do not have Git pre-installed, you should be able to install it with your package manager commands such as `sudo apt-get install git` or `sudo pacman -S git`.

For Mac users, you can install Git via Homebrew with `brew install git`, or you can download the executable installer from Git's website.

For Windows, you can download the executable installer from Git's website. Or, if you have set up Chocolatey, you can run `choco install git.install` in PowerShell. Note that on Windows, you may also want to download Git Bash so you have a Unix-like shell environment available.

To make sure the installation worked, run the `git --version` command again in the terminal.

* **Git Configurations**: `git config` is used to set configuration variables that are responsible for how Git operates on your machine. To view your current setting variables and where they are stored on your system, you can run the following command:

```
git config --list --show-origin
```

Right now you should be seeing only system-level configuration settings if you just installed Git for the first time.

To set your user name, you can run the following command:

```
git config --global user.name "Jane Doe"
```

The `--global` flag is used here to set the user name for all projects on your system that use Git. If you need to override the user name for a particular project, then you can run the command in that particular project directory without the `--global` flag.

To set the user email address, you can run the following command:

```
git config --global user.email janedoe@example.com
```

Another configuration you can set is the preferred editor you want Git to use. Here is an example of how to set your preferred editor to Emacs:

```
git config --global core.editor emacs
```

If you choose not to set a preferred editor, then Git will default to your system's default editor.

Open vs. Closed Source Software
-------------------------------

* **Definition**: "Open-source" means people can see the code you publish, propose changes, report issues, and even run a modified version. "Closed-source" means the only people who can see and interact with the project are the people you explicitly authorize.

GitHub
------

* **Definition**: GitHub is a cloud-based solution that offers storage of version-controlled projects in something called "repositories", and enables collaboration features to use with those projects.
* **GitHub CLI**: This tool is used to do GitHub-specific tasks without leaving the command line. If you do not have it installed, you can get instructions to do so from GitHub's documentation - but you should have it available in your system's package manager.
* **GitHub Pages**: GitHub Pages is an option for deploying static sites, or applications that do not require a back-end server to handle logic. That is, applications that run entirely client-side, or in the user's browser, can be fully deployed on this platform.
* **GitHub Actions**: GitHub Actions is a feature that lets you automate workflows directly in your GitHub repository including building, testing, and deploying your code.

Common Git Commands
-------------------

* **`git init`**: This will initialize an empty Git repository so Git can begin tracking changes for this project. When you initialize an empty Git repository to a project, a new `.git` hidden directory will be added. This `.git` directory contains important information for Git to manage your project.
* **`git status`**: This command is used to show the current state of your working directory - you will be using this command a lot in your workflow.
* **`git add`**: This command is used to stage your changes. Anything in the staging area will be added for the next commit. If you want to stage all unstaged changes, then you can use `git add .` The period (`.`) is an alias for the current directory you are in.
* **`git commit`**: This command is used to commit your changes. A commit is a snapshot of your project state at that given time. If you run `git commit`, it will open up your preferred editor you set in the Git configuration. Once the editor is open, you can provide a detailed message of your changes. You can also choose to provide a shorter message by using the `git commit -m` command like this:

```
git commit -m "short message goes here"
```

* **`git log`**: This will list all prior commits with helpful information like the author, date of commit, commit message and commit hash. The commit hash is a long string which serves as a unique identifier for a commit.
* **`git remote add`**: This command is used to setup the remote connection to your remote repo.
* **`git push`**: This command is used to push up your changes to a remote repository.
* **`git pull`**: This command is used to pull down the latest changes from your remote repository into your local repository.
* **`git clone`**: This command will clone a repository. This means you will have a copy of the repository. This copy includes the repository history, all files/folders and commits on your local device.
* **`git remote -v`**: This command will show the list of remote repositories associated with your local Git repository.
* **`git branch`**: This command will list all of your local branches.
* **`git fetch upstream`**: This command tells Git to go get the latest changes that are on your upstream remote (which is the original repo).
* **`git merge upstream/main`**: This command tells Git to merge the latest changes from the `main` branch in the upstream remote into your current branch.
* **`git reset`**: This command allows you to reset the current state of a branch. Passing the `--hard` flag tells Git to force the local files to match the branch state. This ensures that you have a clean slate to work from.
* **`git rebase`**: A rebase in Git is a way to move or combine a sequence of commits from one branch onto another.

Working with Branches
---------------------

* **Definition**: A branch in Git is a separate workspace where you can make changes. The `main` branch will often represent the primary or production branch in a real world application. Developer teams will create multiple branches for new features and bug fixes and then merge those changes back into the `main` branch.
* **Creating a New Branch**: To create a new branch you can run the following command:

```
git branch feature
```

To checkout that branch, you can run the following command:

```
git checkout feature
```

Most developers will use the shorthand command for creating and checking out a branch which is the following:

```
git checkout -b new-branch-name
```

A newer and alternative command would be the `git switch` command. Here is an example for creating and switching to a new branch:

```
git switch -c new-branch-name
```

* **Branching Strategies**: Your `main` branch is your default branch and usually is pretty stable. So it is best to branch off from there to create new branches for items like bug fixes, new features, or other miscellaneous work.
* **Merge Conflicts**: This happens when Git tries to automatically merge changes from different branches but can't decide which changes to keep. This usually happens when there are conflicting changes for the same portion of the file.

Five States for a Git Tracked File
----------------------------------

* **"Untracked"**: This means that the file is new to the repository, and Git has not "seen" it before.
* **"Modified"**: This file existed in the previous commit, and has changes that have not been committed.
* **"Ignored"**: You likely won't see ignored files in Git, but your IDE might have an indicator for them. Ignored files are excluded from Git operations, typically because they are included in the `.gitignore` file.
* **"Deleted"**: A deleted file is the opposite of an untracked file - it's a file that previously existed, and has been removed.
* **"Renamed"**: A renamed file is a file where the contents are unchanged, but the name or location of the file was modified. In some cases, a file can be considered renamed even if it has a small amount of changes.

`.gitignore` Files
------------------

* **Definition**: The `.gitignore` file is a special type of file related to Git operations. The name suggests that this file is used to tell Git to ignore things, and that's the common use case. But what it actually does is it tells Git to stop tracking a file.

Working with Repositories
-------------------------

* **Definition**: A repository is like a container for a project - if you are working on an app, you would keep the files for that app together in a repository. Repositories can be local on your computer, or remote on a service like GitHub.
* **Public vs. Private Repositories**: A public repository can be viewed and downloaded by anyone. A private repository can only be accessed by you, and anyone you grant explicit access to.
* **Creating Repositories on GitHub**: To create a new repository on GitHub, you can click on the `"New Repository"` button and walk through the GitHub UI of setting up a new repository.
* **Pushing Local Repositories to GitHub**: If you have a local project on your computer, you can push up that repository to GitHub. Here is a step-by-step overview of the process:

1. Initialize an empty git repository in the project directory (`git init`).
2. Make changes to your project.
3. Run the `git status` command to see all changes made that are being tracked by git.
4. Stage your changes (`git add`).
5. Commit your changes (`git commit`).
6. Setup the remote connection (`git remote add`).
7. Push your changes to GitHub (`git push`).

Pull Requests
-------------

* **Pull Requests**: A pull request is a request to pull changes in from your branch into the target branch. Pull requests are the flow you use when you want to contribute code changes to a project. This approach allows the maintainers of the project to review your changes. They can leave comments, ask questions, and suggest tweaks. Then once the review process is complete, it can be approved and merged into the main branch.

Contributing to Other Repositories
----------------------------------

* **Process**: There are thousands of projects that you can contribute to. Here is the basic process on how to contribute to another repository:

1. Read the contributing documentation
2. Find an available issue to work on
3. Fork the repository
4. Clone your forked copy of the repository
5. Create a new branch
6. Make the changes according to the issue
7. Create a PR (Pull Request)
8. Wait for a review for that PR

Working with SSH and GPG Keys
-----------------------------

* **GPG Keys**: GPG, or Gnu Privacy Guard, keys are typically used to sign files or commits. Someone can then use your public GPG key to verify that the file signature is from your key and that the contents of the file have not been modified or tampered with.

To generate a GPG key, you'll need to run:

```
gpg --full-generate-key
```

* **SSH Keys**: SSH, or Secure SHell, keys are typically used to authenticate a remote connection to a server - via the `ssh` utility. You can also use an SSH key to sign commits.

For an SSH key, you'll run:

```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

`ed25519` is a modern public-key signature algorithm.

* **Signing Commits with GPG Keys**: In order to sign your commits with your GPG key, you'll need to upload your public key, not the private key, to your GitHub account. To list your public keys, you will need to run the following:

```
gpg --list-secret-keys --keyid-format=long
```

Then, to get the public key, use:

```
gpg --armor --export "<key id>"
```

Then, take the short ID you got from listing the keys and run this command to set it as your git signing key:

```
git config --global user.signingkey <your_gpg_key_id>
```

Then, you can pass the `-S` flag to your `git commit` command to sign a specific commit - you'll need to provide your passphrase. Alternatively, if you want to sign every commit automatically, you can set the autosign config to `true`:

```
git config --global commit.gpgsign true
```

* **Signing Commits with SSH Keys**: To sign with an SSH key, which is a relatively new feature on GitHub, you'll need to start by uploading the key to your GitHub account. Then you'll need to set the signing mode for git to use SSH:

```
git config --global gpg.format ssh
```

Then, to set the signing key, you'll pass the file path instead of an ID:

```
git config --global user.signingkey <path_to_your_ssh_keys>
```

---

## Module 4: Advanced Git Workflows, Code Reviews, & CI/CD

### Lecture 4.1: What Is A Gitignore File And What Are Some Items That Should Be Included Inside It

# What Is a .gitignore File, and What Are Some Items That Should Be Included Inside It?

We have briefly touched upon the `.gitignore` file in a previous lesson. But what exactly is this file, and what should you put in it?

The `.gitignore` file is a special type of file related to Git operations. The name suggests that this file is used to tell Git to ignore things, and that's the common use case. But what it actually does is it tells Git to stop tracking a file. This distinction is important, and will be clarified later.

What should you actually put in this file? Well, you should list things that you don't want committed.

The first would be your secrets files. This may be something like a `.env` file, where you've stored your API keys for your application to consume. It may be a private GPG key file that your app needs to use for authentication. Anything that contains sensitive information you would not want leaked to the public should be ignored with `.gitignore`. Even if your repository is private, you should act as if it is public - treat it like anyone can see it, and take care not to commit secrets.

Let's take a look at what our file might look like right now:

```
# Secrets
.env
github.key
```

We've told Git to ignore the `.env` file, where we are keeping our secrets. We've also told Git to ignore a `github.key` file, which contains a private GPG key.

The next thing to consider are the packages, or dependencies, that your project uses. As an example, when you are working with a Node.js project, you probably install packages from npm. These packages go into a `node_modules` folder in your project, so your code can import and consume them.

But the `node_modules` folder gets prohibitively massive, and you definitely don't want to commit all of those packages and track the changes each time you update one. Instead, you commit your `package.json` file, and the relevant lockfile (e.g. `package-lock.json`, `pnpm-lock.yaml`). These files tell npm what packages and versions to install, so a contributor can install the same dependencies you are using without having to commit them to the repository.

Let's go ahead and add `node_modules` to our `.gitignore` file:

```
# Secrets
.env
github.key

# Packages
node_modules
```

Now, let's touch on an important syntax thing for `.gitignore` files. When you add an entry like `node_modules`, Git will ignore anything that matches that pattern. This means it will ignore the `node_modules` directory in the root of your project, but would also ignore the `node_modules` in the `client` directory of your project.

If you only want to ignore something at the root, you can prefix the line with a forward slash. `node_modules` would become `/node_modules`. This would ignore the root `node_modules` directory, but not the `client/node_modules` directory. We do not want that, so let's leave our entry as just `node_modules`.

The next thing you want to consider ignoring are your build outputs. For example, compiling a TypeScript project might result in a `dist` folder for the JavaScript output. You don't want to commit that output, because it bloats the Git history. Instead, you want to ignore that output - contributors can reproduce it for themselves by running the same build command.

Let's go ahead and ignore the `dist` folder:

```
# Secrets
.env
github.key

# Packages
node_modules

# Outputs
dist
```

Sometimes, a misplaced file can cause the TypeScript compiler to break, which results in our JavaScript output ending up all over the place. Since we are exclusively writing TypeScript, let's go ahead and use glob syntax to ignore all JavaScript files:

```
# Secrets
.env
github.key

# Packages
node_modules

# Outputs
dist
*.js
```

Some other common outputs you might ignore are the `coverage` directory, for the results of unit test coverage, an `.angular` directory if you are using Angular, a `.next` directory if you are using NextJS, and so on.

For now, we can stick with what we have here. If you're using a framework that generates files, you should confirm in their documentation what you need to add to the `.gitignore`.

The fourth batch of things to ignore are IDE files. Jetbrains products, for example, might use an `.idea` folder for IDE-specific configurations. Visual Studio Code uses a `.vscode` folder.

These are often good to ignore, because they'll contain files specific to your local environment that other contributors won't need (because they use their own configurations). Let's go ahead and add the Visual Studio Code directory, since that is what we are using as our IDE.

```
# Secrets
.env
github.key

# Packages
node_modules

# Outputs
dist
*.js

# IDE
.vscode
```

But our `.vscode` folder does contain a `settings.json` file, which includes some workspace-specific stuff that might be useful for our contributors - this file allows them to configure their extensions and environment to better mirror our own.

So let's go ahead and use negation syntax to "unignore" that file:

```
# Secrets
.env
github.key

# Packages
node_modules

# Outputs
dist
*.js

# IDE
.vscode
!.vscode/settings.json
```

If you are on MacOS, you may be familiar with the `.DS_STORE` file. This file contains metadata that Finder uses to determine things like how to render the directory (e.g. with thumbnails, or as a list). Similarly, Windows users might see a hidden `Thumbs.db` file, which caches thumbnails for the directory.

It's generally a good idea to ignore these files, since they're a personal setting that have no impact on the project. Let's add both of them:

```
# Secrets
.env
github.key

# Packages
node_modules

# Outputs
dist
*.js

# IDE
.vscode
!.vscode/settings.json

# System Files
.DS_STORE
Thumbs.db
```

A quick note about ignoring previously committed files. Say you've accidentally committed your `dist` directory earlier, but now you want to remove it and ignore it. You cannot just add it to your `.gitignore` file - this does not make previously committed content disappear, it tells Git to stop tracking the file. So if you ignore a file that's already committed, Git won't track any changes but it also won't track the deletion of the file.

Instead, you'll first need to delete the file. Create a commit with that deletion. Then you can add the item to your `.gitignore` and create a second commit with that update. Going forward, when that file is created again, Git will ignore it and it won't show up in your commits.

Finally, if you're working on a project in a different language, such as Python, the items you need to ignore will be different than what we've covered here. GitHub maintains a very helpful repository of `.gitignore` templates for various languages and frameworks. You can find that list at <https://github.com/github/gitignore>.

With that, you're now ready to avoid committing files you don't want in your repositories!

---

### Lecture 4.2: What Are Some Best Practices For Developing A Git Branching Strategy

# What Are Some Best Practices for Developing a Git Branching Strategy?

We've talked a bit about branches in the previous lessons. You've learned how to create branches, why you shouldn't commit directly to `main`, and similar. But when and why should you actually create branches?

First, let's talk about why you shouldn't just push a bunch of commits to `main`. Your default branch should be reliably stable - that is, at any given time I should be able to pull down your current `main` branch and build, run, and test your application. If you are pushing up partially completed features, or WIP commits, then this may not always be true.

Additionally, it is very common to work on multiple features in tandem. If you're pushing partial work to `main` for multiple features simultaneously, it becomes much more challenging to debug a potential issue since you do not have isolated changes. On top of that, context switching (or changing which tasks you are working on) is nowhere near as clean.

So when should you create a branch? A general rule of thumb is to create a branch for every isolated unit of work. That is, if you are working on a new OAuth feature, that work should be on a dedicated branch. If you then need to fix a bug in your password authentication, that work should be on its own dedicated branch. Need to redesign the user profile page? That's another branch.

Note that you should always create your branches off of `main`. So, if you are working on a branch for your OAuth feature, you would checkout `main` before creating a new branch for your password authentication fix. Otherwise, if you create a branch for the password fix directly from your OAuth branch, you'll end up with the commits from your OAuth work and the history will be muddied.

But how should you name your branches? Well, that's entirely up to you (or the project you are contributing to), but here are a few common conventions:

`scope/description` - where `scope` is something like `feat` or `fix`, and `description` is a very short explanation of the branch's changes. For example: `feat/oauth-support`.

`scope/issue/description` - similar to the previous convention, but including the number associated with the related issue. For example: `fix/25/password-auth`.

`username/scope/description` - For projects where you all work off of branches in the original repository instead of forking it (this is common with private internal repositories), it can be helpful to include your username at the start of the branch. For example: `naomi-lgbt/feat/profile-redesign`.

Let's cover a few other notes about branching strategies.

For long-lived feature work, such as a beta feature that requires significant developer-hours, you may want to use a feature flag to selectively enable the logic rather than a branch. The longer a branch remains unmerged, the more likely you are to encounter conflicts.

You may, however, wish to maintain dedicated branches for deployment environments or releases. For example, the freeCodeCamp repository uses `prod-staging` and `prod-current` to trigger deployments to staging and production servers, respectively. This can free up the team to iterate faster, merging as things are ready and approved without having to trigger a deployment for every merge. Instead, deployments are created by merging the latest `main` into those production branches.

You may also want to maintain "release branches", or branches that represent a major version of your product. This allows you to have a clean state for each major release, so if you need to backport a critical security patch to an earlier release version you can do so without having to include any of the new version's changes.

And finally, you should avoid merging your branches into `main` using the local CLI. Instead, create a pull request with your changes and merge through that flow. This gives you a chance to ensure any tests pass in your CI (which you will learn about in a future lesson), and to double check the diff view to make sure you have included only the changes you want merged.

With these tips, you can start branching your way to success!

---

### Lecture 4.3: What Are Good Practices For Remaining In Sync With Your Remote Counterparts

# What Are Good Practices for Remaining in Sync with Your Remote Counterparts?

We've talked a bit about using branches to work on isolated changes to avoid soiling your `main` branch. But what does that mean, and why is it important?

If you commit changes directly to your `main` branch, and the upstream repository accepts other changes that are not yours, you will end up with something called a "divergent history". This means that the commits on your `main` branch are no longer aligned with the commits on the upstream `main` branch. And it makes syncing the upstream changes a nightmare.

So, let's say you've been following good branching practices, and this isn't an issue. If you followed along with our previous lessons, you should have a fork of a repository that you've cloned locally, and you should have an upstream remote that points to the original repository.

If you did not do this, here's a quick reminder. You'll want to fork a repository, clone your fork locally, and run this command:

```
git remote add upstream <url>
```

Replace `<url>` with the SSH URL for the original repository, NOT your fork.

With a properly configured upstream, you can run the following series of commands to pull in the latest upstream changes:

```
git checkout main
git fetch upstream
git merge upstream/main
```

What do these do? Well, you've learned about `git checkout`, so the first command ensures that you are on your `main` branch locally.

The second command, `git fetch upstream`, tells Git to go get the latest changes that are on your upstream remote (which is the original repo). However, unlike a pull, Git will not automatically update your branch. This is important, because your `main` branch locally is connected to the `main` branch on your fork - not the `main` branch on the original repo! Performing a git pull may result in unexpected behavior.

The final command, `git merge upstream/main`, tells Git to merge the latest changes from the `main` branch in the upstream remote into your current branch - which is your local `main` branch, because that's what we checked out.

But what if the merge fails? What if you've accidentally committed to `main`, and Git cannot merge the divergent histories? Well... assuming you have not made any pull requests from your `main` branch, you can do a hard reset to force Git to update your branch.

```
git reset --hard upstream/main
```

The `git reset` command allows you to reset the current state of a branch. Passing the `--hard` flag tells Git to force the local files to match the branch state. This ensures that you have a clean slate to work from. And passing `upstream/main` tells Git you want your current branch (which is `main`) to match the `main` branch of the upstream remote. Be cautious with this command - any time you forcibly update a Git history, weird and unfortunate things may happen.

Once you've got your local `main` branch updated correctly, it's important to push that state up to your remote fork (which should be `origin`, if you have followed our lessons). To do this, you can run:

```
git push
```

This will push the current state up to your remote fork. But if you've had to do a hard reset to clean up the history, it's possible your remote fork also has a divergent history and the push will fail.

You can rectify that by forcing the push:

```
git push --force
```

**Be careful with this command**. Doing a force push effectively rewrites your remote history, and if you've done something incorrectly then a forced push becomes a nightmare to untangle.

Pushing the synced changes up to your remote fork is important because it helps you ensure that you can safely clone the fork with the latest changes if you've lost your existing local repository.

And once you've got your `main` branch synced, you are free to create a new branch from that state to start working on another contribution - with the latest version of the original codebase!

---

### Lecture 4.4: What Are Merge Conflicts And How Can You Resolve Them

# What Are Merge Conflicts, and How Can You Resolve Them?

If you've been around experienced developers, whether in an online community or in person, you have probably heard about the "dreaded merge conflicts". But what exactly are they?

Well, when you are using a proper branching strategy like we've discussed in previous lessons, you may be working on two different features on two different branches at the same time. Or maybe you're working on something, and a colleague is working on another branch. Either way, you have two independent changes going on. But sometimes, both of those branches will edit the same file. And if the other branch gets merged into `main` first, your branch's changes are now behind.

Most of the time, this can be fixed by merging `main` back into your feature branch. But when the changes from the other branch conflict with your branch, Git cannot tell which changes you want to keep during a merge. This is called a "merge conflict".

But how can you fix it? Well, for smaller and simpler conflicts, GitHub will give you a web UI to fix it. A "Resolve conflicts" button will show up at the bottom of a PR if there's conflicts. If you click it, you will see the file with conflicts that includes your code and the conflicting code. Git will add "merge conflict markers" around your code and the conflicting code to help identify the issue. It looks something like this:

```
1 <<<<<<< feat/conflict
2 Here's some code from my first PR :)
3 =======
4 Here's some code that was merged to main that conflicts with the code on my PR
5 >>>>>>> main
```

The opening marker is the `<<<<<<< feat/conflict`, and indicates the start of the changes that our current branch is making. Then we see the `Here's some code from my first PR :)`. After that is the `=======` marker, which indicates the end of our changes and the start of the `main` branch's changes. We can see that the changes made on `main` are the line `Here's some code that was merged to main that conflicts with the code on my PR`. And after that is the closing `>>>>>> main` marker to show the end of the conflicts.

But how do we fix it? Well, you need to decide which changes you want to keep as part of the merge conflicts. If you want to keep both changes, you could remove just the conflict markers and leave the changes unchanged. Alternatively, if you want to keep the changes from only one branch, you would delete the conflict markers and the changes from the other branch (those that you do not wish to keep). And finally, if you don't like any of the changes at all, you can remove everything from the opening marker to the closing marker (inclusive).

Let's remove the `main` branch changes, but keep ours. Here's what we have now:

```
1 Here's some code from my first PR :)
```

Click the "Mark as resolved" button, which tells GitHub you are satisfied with your resolution. If there were additional files, GitHub would switch to the next one. But since this is our only conflicted file, you'll see a "Commit merge" button appear. Click that button and GitHub will create a merge commit for you. You'll be taken back to the pull request, where you'll see your new merge commit and the conflicts resolved. And we're all set!

But what if you can't edit the conflicts directly on GitHub, because they are too complex?

Well, if your branch has few commits, or only a couple of commits modify that file, you may be able to merge `main` into your branch:

```
git checkout feat/conflict
git fetch origin
git merge origin/main
```

As Git processes this merge, you'll get conflicts to resolve manually. Git will notify you of which files need to be fixed. When we open the files with conflicts in our editor, we get the same conflict markers, with some helpful UI additions thanks to VSCode. Go ahead and fix the conflicts in the file in the same way. But this time, we'll need to manually create the commit. It's the same as creating any other commit:

```
git add .
git commit -m "chore: resolve conflicts"
```

After running these commands, we can see Git has accepted our resolution.

Sometimes, when you have many commits or conflicts, a rebase can be helpful. Instead of merging changes, a rebase takes all the commits on your branch and reapplies them so they come after the latest changes on `main`. In Git terms, this effectively "resets" the base of your branch to the most recent commit on `main`.

In order to experiment with this, we need a new branch:

```
git checkout main
git pull
git checkout -b feat/rebase
```

Let's go ahead and generate a bunch of commits for our branch, so we can practice rebasing:

```
echo "change one" > README.md
git add .
git commit -m "change one"
echo "change two" > README.md
git add .
git commit -m "change two"
echo "change three" > README.md
git add .
git commit -m "change three"
```

Now, let's go make another change on `main` to create a conflict:

```
git checkout main
echo "change four" > README.md
git add .
git commit -m "change four"
```

And checkout our rebase branch:

```
git checkout feat/rebase
```

Next, run `git rebase -i main`. It will rebase our branch onto the current state of the `main` branch. The `-i` flag tells Git to perform a rebase in interactive mode. You will see your commits with the word `pick` next to them. `pick` tells Git to use the commit as-is for the rebase. Save and close the file, and we'll get an error message telling us there is conflicts.

Our `change one` commit conflicts with the `change four` commit, and we need to resolve that. Open the file in your editor, and you'll see the same UI as we got with the conflicts earlier. Let's keep our `change one` changes. Then, you'll need to run `git add .` to add the changes, and `git rebase --continue` to tell Git we're ready to continue rebasing. Since we've resolved the conflict in the first commit, Git can automatically handle rebasing the rest of the commits.

Now, just as a last bit of cleanup, let's squash our three change commits into one single commit for a cleaner history. Run `git rebase -i main` again to get to the editor. Then, leave the first command as `pick` but change the next two to `squash`. You may run in to the same conflict again. If you do, resolve it the same way you did before. Once you've resolved and continued the rebase (or immediately, if you had no conflict), you'll see a new commit message editor pop up. This message will be your new commit, containing the changes from the three commits we've squashed. Let's name this one `change three complete`. Save and close the editor, and Git will finalize the rebase.

If we check your commit history now, we can see that we now have our single `change three complete` commit, and it's correctly based on the `change four` commit. That means you've successfully completed a rebase with squashed commits! And now you've got the tools you need to become a merge conflict champion!

---

### Lecture 4.5: What Does A Typical Code Process Look Like For Projects

# What Does a Typical Code Review Process Look Like for Projects?

In a previous lesson, you learned how to make a pull request to your own repository. You also learned how to merge that pull request. But you could only do that because the repository belongs to you - you have maintainer access to your own repositories, which means you have permission to merge pull requests.

When you contribute to someone else's open source project, however, you typically won't have those permissions. Instead, you'll need to wait for the maintainers to go through the code review process and accept your contribution. They will then handle merging it.

But what does the code review process look like?

The process that maintainers take will vary from person to person, and there may be project-specific approaches. But in general, there are typically three steps to a code review.

The first is to confirm that the CI, or continuous integrations, passes. You'll learn more about this in a future lesson, so for now you can think of them as checks to validate that the code meets style guidelines and passes a test suite.

If the CI fails, maintainers will typically request that you update the pull request to address the failures. These failures should include some sort of report you can look at to see what went wrong, but maintainers may also provide you more specific guidance to resolve the issue.

Once the checks pass, the maintainers will look at your actual code changes. They can analyze the diff view to see what you've modified, added, or deleted. They may ask questions about why you took specific approaches, so it's good to be deliberate and thoughtful when you are preparing conversations.

They may also request you make additional modifications. We'll talk about what that looks like in a bit.

The last step is usually to pull down your changes locally. The maintainers can then run the application with your modifications, test the functionality, and verify nothing is broken or behaving in unexpected ways.

If everything looks good, a maintainer will approve your pull request - sometimes with a "LGTM" comment, which stands for "looks good to me". After your pull request has been approved, it should be merged whenever the maintainers are ready to pull the changes in. Some projects may require more than one approval - freeCodeCamp, for example, requires two.

But what if something is not correct with your pull request? Maintainers can perform a review in which they request changes. These requests can come in a couple of forms.

Sometimes, a maintainer may just leave a "comment" with their request, maybe indicating something you should change or update, but with more freedom of how you implement it.

Or, maintainers may also leave an official "request changes" comment. Typically, a comment like this blocks the pull request from being merged. You'll need to make the desired changes, and then the same maintainer who requested the changes will need to re-review and request more changes or approve your work.

When maintainers have specific changes in mind, they can actually propose changes through GitHub's UI. When they use a direct suggestion like this, GitHub will give you a button to commit the suggestion to your branch directly. However, if there are multiple suggestions like this, you'll want to switch to the files view.

From this view, you can add all of the suggestions (one by one) into a "batch", and commit them all in one go. This is incredibly useful when there are many suggestions, as doing them individually would result in many commits. All of the CI checks would have to run on each and every commit, and this can slow down the process for accepting your PR.

If the requested changes are significant, you will likely want to make the changes locally, commit them to the same branch that you used for the PR, and push them up. GitHub will automatically update your pull request to reflect the new commits.

There are a couple of other notes that we want to cover.

First, remember that maintainers are people too. Open source projects rarely generate enough revenue for maintainers to work on them full time, which means they have to keep a job. It is important to be patient with the review process - don't do things like ping maintainers repeatedly for a re-review, or try to rush them in their review process.

Making contributions can be exciting! But don't rush through the process. Instead, take your time. Make sure to test your changes locally - run any test suites the project may have, run the development server and manually confirm that your changes work, etc. And always follow the contribution guidelines for the specific project you are working on.

If you keep all of that in mind, and put your best effort forward, your contributions should go smoothly and your code review should be a solid approval!

---

### Lecture 4.6: What Is Ci Cd And How Does Ci Work With Github Actions

# What Is CI/CD, and How Does CI Work with GitHub Actions?

CI stands for Continuous Integration, and CD stands for Continuous Delivery or Continuous Deployment. Together, these processes allow you to automatically deploy changes to your application after ensuring those changes are functional.

In a CI pipeline, you might run your linter and tests against the code. CI pipelines typically run on pull requests to ensure the changes made aren't breaking the app, and also on the `main` branch to ensure it is ready to deploy.

A CD pipeline might also run on pull requests, if you set up a preview environment so you can look at the changes live. But you'll also run it on your `main` branch to continuously deploy changes as they are accepted and merged.

But how do these actually work with GitHub Actions? First, we need to understand what GitHub Actions actually are. GitHub Actions provides ephemeral runners (think like a temporary computer) that allows you to execute specific commands.

Actions are configured with a YAML file. You can have multiple files to specify different actions to run. For example, you might have one file for your CI and another for your CD.

Let's take a look at a basic CI example:

```
name: Node.js CI
on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main

jobs:
  lint:
    name: Lint and Test
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Source Files
        uses: actions/checkout@v4

      - name: Use Node.js v22
        uses: actions/setup-node@v4
        with:
          node-version: 22

      - name: Setup pnpm
        uses: pnpm/action-setup@v2
        with:
          version: 10

      - name: Install Dependencies
        run: pnpm install

      - name: Lint Source Files
        run: pnpm run lint

      - name: Verify Build
        run: pnpm run build

      - name: Run Tests
        run: pnpm run test
```

This is a lot, so let's break it down. Looking at the first section:

```
name: Node.js CI
on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main
```

The `name` defines the name of the action itself. This appears in areas like the status checks section of a PR. The `on` properties define what's called "workflow triggers" - these are the events that will trigger your action to run.

In this example, we run the action when commits are pushed to `main`, and when a pull request targets `main`. This means the CI runs when someone makes a pull request, and again when we merge it.

The `jobs` section is where you define what your action actually does. The `lint:` key is an arbitrary key that defines the internal name for that job. The `name` property defines the external name for this particular job. And the `runs-on` property defines what kind of environment your action should run in - for this case, we're running it in the latest supported version of Ubuntu.

The `steps` property is where the magic happens. This block defines the actual steps your action should take. Let's take a look at the first block there:

```
      - name: Checkout Source Files
        uses: actions/checkout@v4
```

This step has two properties, the `name` the step should have, and a `uses` property. This `uses` property is special, in that it tells the action runner to go get a public action from GitHub and run it, instead of running a command. The `actions/checkout` action handles cloning and setting up the repository within your runner.

```
      - name: Use Node.js v22
        uses: actions/setup-node@v4
        with:
          node-version: 22

      - name: Setup pnpm
        uses: pnpm/action-setup@v2
        with:
          version: 10
```

The next two blocks also use third-party actions. These steps set up Node and the pnpm package manager. Both of them have a `with` key, which you can use to pass arguments to those third party actions. Think of this as like passing arguments to a function.

The final four blocks are where the magic really happens.

```
      - name: Install Dependencies
        run: pnpm install

      - name: Lint Source Files
        run: pnpm run lint

      - name: Verify Build
        run: pnpm run build

      - name: Run Tests
        run: pnpm run test
```

We have an `Install Dependencies` block, which installs the npm packages. Our `Lint Source Files` block runs the linter, the `Verify Build` block ensures that the TypeScript code can compile, and the `Run Tests` block runs the unit tests.

The important thing to know about actions is, by default, if one of these steps fails the remaining ones will be skipped and the entire run will be marked as a failure.

Where do you put your YAML files so you can run these actions? They need to go in a `.github/workflows` directory in your repository for GitHub to find and consume them.

There are a lot of additional things actions can do, and I encourage you to read the documentation and explore existing actions in projects like the freeCodeCamp repository. But for now, you should have a decent understanding of the basics of GitHub Actions and CI/CD!

---

### Lecture 4.7: How Do You Use Github Pages To Deploy A Project

# How Do You Use GitHub Pages to Deploy a Project?

GitHub Pages is a really solid option for deploying static sites, or applications that do not require a back-end server to handle logic. That is, applications that run entirely client-side, or in the user's browser, can be fully deployed on this platform.

Additionally, GitHub Pages are completely free for open source projects. There are plenty of good reasons to make your project open source, and Pages adds yet another.

But how do you actually deploy to GitHub Pages? Well, that depends on how your application works.

Let's start with a basic HTML page. Here's one you can add to your existing repo if you'd like:

```
<!DOCTYPE html>
<html>
  <head>
    <title>freeCodeCamp</title>
    <link rel="stylesheet" href="./style.css" />
  </head>
  <body>
    <h1>Welcome to freeCodeCamp's Lessons!</h1>
    <p>Let's have some fun learning about Git and GitHub!</p>
  </body>
</html>
```

Now we need to visit our repository and click the "Settings" tab to go to the repository settings. Then we need to select "Pages" from the sidebar.

There's only a few options initially, but that's going to change as we start configuring the settings. First, we need to tell GitHub what to deploy from.

We'll want to leave this as "Deploy from a branch", because we aren't using a framework and have not configured any GitHub actions at all. You'll learn more about what those are in an upcoming lesson.

Next, set the branch that we are deploying from to `main` to deploy what's on that.

You'll then get a choice to deploy from your project's root folder or from a `docs` folder. This feature is used by projects like freeCodeCamp - we used to bundle documentation with our app, so we could deploy just the documentation onto GitHub pages via the `docs` folder. For now, leave it as the `/` (root) folder and hit the "Save" button next to this drop down to save your changes.

Once you've saved, you'll see a new input to configure a custom domain. If you have one already, and would like to use it, you can follow the link to the docs to do so. For this lesson, however, we are going to leave this blank.

You can also see the domain that your new GitHub Pages site has been deployed to. Without a custom domain, this defaults to `<username>.github.io`, where `<username>` is the name of your account (or the organization's account if you are deploying from an org-owned repository). And repository will be served on a path matching the repository's name, `<username>.github.io/<repo-name>`, for instance. If you visit the URL, you will see your site!

Now, when you push new changes to your `main` branch, GitHub Pages will automatically update our deployed site with the latest changes. This process can take a few minutes, depending on server load - and you may need to do a hard refresh to clear the cache.

And with that, we have successfully deployed a basic web application to GitHub Pages. You can also include CSS and JavaScript files in your Pages deployment, so you can build beautiful and interactive sites. And once you learn a framework like React or Angular, you can even deploy those on GitHub Pages too!

---

## Module 5: Relational Database Fundamentals & SQL

### Lecture 5.1: What Are Relational Databases And How Do They Differ From Non Relational Databases

# What Are Relational Databases, and How Do They Differ from Non-Relational Databases?

A relational database is a collection of data organized into tables. These tables are made of rows and columns.

Rows represent individual records. For example, if you're storing user data, each row could represent a specific user.

Columns represent the attributes or fields that describe each record. The table might include columns for common user attributes, such as name and national ID number.

One of the key characteristics of relational databases is that they allow us to connect different pieces of information by linking tables through common attributes, making it easier to see how they relate to each other.

Relational databases require a schema. The schema defines the overall structure of the database, including its tables, columns, data types, relationships, and constraints.

All tables in a relational database have a primary key, which is a unique identifier for each row. They enable relationships between tables via foreign keys. You'll learn more about primary keys, foreign keys, and how they work in the coming lessons. For now, just know they are fundamental to linking records across tables.

For example, let's say that you're creating a database for an organization that runs a wildlife conservation center for critically endangered animals.

One of the tables could store general information about the animals, you might call it `animals`. Each row could represent an animal, while each column could represent an attribute of that animal, like species, size, weight, age, and other unique characteristics.

To uniquely identify each animal, you would typically add an `id` column to the table. This would be the primary key of the table because it's unique for each animal. The ID of each animal could be used to link its record in this table to related records in other tables.

You could also have a `species` table to store information about each species, such as their habitat and conservation status. Each animal in the `animals` table could reference a species from this table using a species ID.

You could also create a table to store the veterinary records of the animals. This way, the center can track their health, treatments, and medications.

Once you have this general schema, you could link these tables to the `animals` table, which acts as the central point for animal-related data.

This way, you don't have to keep all the information about an animal in the same table. Instead, you can store related data in separate tables and link them through relationships. By creating these relationships, you can get the specific data you need with a single query.

A query is a request for specific data from the database. Examples of queries that you could make in the context of our example would be finding all animals that need a veterinary checkup, finding the most critically endangered species in the center, finding the number of animals who were born in captivity, and more. You can customize the queries to fit your needs.

Our example was related to wildlife conservation, but relational databases have a wide range of applications across industries such as healthcare, construction, business, gaming, education, government, e-commerce, social media, and more.

They offer several advantages, including scalability. They can handle large datasets, so they're perfect for complex, real-world applications. They also enforce data integrity through primary keys, foreign keys, and data types, which ensures that the data will be consistent and accurate.

In addition to relational databases, you can work with non-relational databases.

The main difference between relational and non-relational databases is how the data is stored. Non-relational databases, also known as NoSQL databases, are more flexible. They store data in individual files that are not connected. Their data model is more flexible too.

While some non-relational databases may have a basic schema or data model, it is often less rigid than the schema defined in relational databases. You can add, modify, or remove data fields if necessary.

The decision to use a relational or non-relational database depends on various factors, including the nature of the data and the specific requirements of the application. You should evaluate the tradeoffs between these two approaches to choose the best one for your application.

---

### Lecture 5.2: What Are Some Common Relational Databases And How Do You Install And Use Postres

# What Are Some Common Relational Databases, and How Do You Install and Use Postgres?

Relational databases have a wide range of applications, including web development, inventory management systems, healthcare systems, e-commerce applications, and more.

Some of the most common relational databases are MySQL, PostgreSQL, SQLite, and Microsoft SQL Server. Let's learn a little bit about each one of them.

MySQL is an open-source relational database management system. It's very popular for web development because it's easy to use, reliable, and efficient for building real-world applications. It also has an active community of developers that support and maintain it.

PostgreSQL is officially described as "The World's Most Advanced Open Source Relational Database." It's a free, open source object-relational database system known for its reliability, data integrity, and extensibility. For example, you can define your own data types, custom functions, and write code in different programming languages without re-compiling your database.

SQLite is a free, open source, and lightweight file-based SQL database engine. It's one of the most widely used database engines in the world. SQLite is self-contained and serverless. It's a zero-configuration database, which means that it doesn't require an initial setup process, which is great for getting started quickly.

These three databases are free and open source. There are other popular proprietary options too, including Microsoft SQL Server and Oracle database.

Microsoft SQL server is a popular relational database management system developed by Microsoft and used in various applications.

Oracle database is a scalable relational database management system often used for enterprise applications that require high performance.

Great. Now that you know more about the different options available, let's see how you can install PostgreSQL.

First, you need to go to the official website: <https://www.postgresql.org/>.

Once you're there, click on the "Download" button.

This will take you to a page where you can select your operating system. If you click on one, you will be taken to the instructions for that OS.

We will go through the installation process for the Windows operating system, but the process is similar across operating systems.

From this page, you can download the installer by clicking on the "Download the installer" link.

This will take you to a page where you can choose the version of PostgreSQL you want to install. If you click on the corresponding icon, the download should start.

Then, in your Downloads folder or the folder where you store your downloads by default, you should see the installer.

If you double-click on it, you will start the setup process. Click Next.

Choose the directory where PostgreSQL will be installed. You'll see one by default but you can customize it.

Then, select the component that you want to install. There are four possible components:

* PostgreSQL Server, the database engine itself.
* pgAdmin 4, a user-friendly tool for database management.
* Stack Builder, a tool for downloading and installing additional PostgreSQL-related software and extensions
* And Command Line Tools, to interact with the PostgreSQL server directly from your terminal. This includes psql, an interactive terminal for executing SQL queries.

When you're ready, click Next.

Then, select a directory to store your data. You will see a default path but you can customize this. When you're ready, click Next.

Now you'll need to enter a password for the database superuser, the user with unrestricted access to all databases and objects. Type in your password, retype it, and then click Next.

Then, select the port number the server should listen on. By default, it's 5432. Then, click Next.

You'll need to choose a locale for the new database cluster. This is important for the database to interpret locale-sensitive data types. Then, click Next.

Finally, you'll see a pre-installation summary. Take a moment to review this and click Next.

You will need to confirm that you want to start the installation process. If you click Next, the process will start. It should only take a few minutes.

When the process is completed, based on the components that you installed, you may have to choose if you want to launch Stack Builder to download and install additional tools, drivers, and applications.

If you decide to launch Stack Builder, you'll see a screen where you can start the installation. Alternatively, you can click Cancel to do this later on.

Congratulations! Now you have PostgreSQL installed on your computer. The process should be similar for other operating systems. After this, you can start using the database.

Go to your apps and search for pgAdmin, an open source administration and development platform for PostgreSQL that should have been installed if you selected it in the components. Click on pgAdmin 4 to open it.

You'll see an initial loading screen when the application starts. Then, you should see a dashboard where you can start a new server, check your databases, configure pgAdmin, and more. You'll also find helpful links to the documentation.

If you click on "Servers" at the top left, you will need to enter the password that you chose during the installation.

After entering your password, you should see a screen where you will have access to your databases, including their tables.

You'll also find another very helpful tool, psql, an interactive terminal for SQL queries. To open it, search for psql on your system. Click on it.

It will open the SQL Shell, where you can start running commands.

And that's how you can install PostgreSQL on Windows. The process is very similar for macOS and Linux.

Alternatively, if you are installing it on macOS, you can use Homebrew, a package manager. Once you have Homebrew installed, run this command to install PostgreSQL:

```
brew install postgresql@<version>
```

You can specify the version that you want to install by writing the number after the at (`@`) symbol.

---

### Lecture 5.3: What Is Sql And How Can You Create A Database With Tables

# What Is SQL, and How Can You Create a Database with Tables?

SQL stands for Structured Query Language. It was developed in the 1970s, when it was initially known as the structured English query language (SEQUEL). This term was later shortened to SQL.

SQL is a programming language used for storing and managing data in relational databases.

Like you learned in a previous lesson, relational databases organize data into tables. Each table has a set of rows and columns, where the data attributes and their relationships are represented. Each row represents a record while each column represents a specific attribute or field of that record.

With SQL, you can add, change, delete, find, and retrieve data from a relational database. It provides a comprehensive set of commands for querying, filtering, sorting, and aggregating data.

SQL can help optimize database performance, by querying only the necessary data, and it can be easily integrated with a wide range of programming languages, so you can use it to interact with databases directly from your applications.

It has been also adopted as an industry standard. It enforces data integrity and includes many security features, like support for user authentication and data encryption.

It's also scalable, portable, and compatible with a wide range of database management systems.

SQL is based on commands, commonly known as SQL statements or SQL queries.

As a developer, you will write these statements using specific SQL language elements or keywords. They allow you to perform the necessary operations on your database.

Before you can enter SQL commands, you need to open the psql shell so you can directly interact with the PostgreSQL database. In the command prompt or terminal, enter:

```
psql -U <username> -d <database_name>
```

Replace `username` with your username and `database_name` with the database you want to connect to.

If you have not created your own database yet, PostgreSQL automatically includes a default database called `postgres` when it is installed. You can use this `postgres` database to follow along.

Once connected, you will see the prompt change to:

```
postgres=#
```

It shows the database name you are connected to and waits for SQL commands.

Let's go over some of the most fundamental SQL commands that you should be familiar with. You'll notice that, by convention, SQL commands end with a semicolon (`;`).

First, you can use this command to create a database named `my_database`:

```
CREATE DATABASE my_database;
```

You can type `CREATE` followed by `DATABASE`, and the name of the database that you want to create. Notice that the SQL keywords of the command are written in capital letters.

Then, once you have your database, you can connect to it.

How you connect to the database really depends on the environment and tool you're using.

In the command prompt or terminal, you can use the method shown earlier. In the interactive psql shell, you can switch databases with the `\c` shortcut command followed by the database name like this:

```
\c my_database
```

Note that the `\c` command and other shortcut commands (ones with a backslash in front of them) are part of the psql shell and not part of the SQL language itself, so they do not require a semi-colon to complete the command.

Now that you've connected to your new database, you will see the prompt has changed:

```
my_database=#
```

Once you have created and connected to a database, you can create a table with the `CREATE TABLE` keywords:

```
CREATE TABLE products (
  id SERIAL,
  name VARCHAR(255)
);
```

In the command, you write `CREATE TABLE`, followed by the name of the table that you want to create. In this case, it will create a table named `products`.

Then, within parentheses, you write the names of the columns that the table should have and specify the data type of the values that will be stored in each column.

In the example, the table will have two columns, a column for the product ID and another one for the name of the product.

The standard naming convention for table and column names is snake case, writing words in lowercase and separating them with an underscore (`_`). For example: `delivery_orders`

These are few essential SQL commands you should know to get started.

With SQL, you can easily query, manipulate, and analyze data to make informed decisions and solve real-world problems.

---

### Lecture 5.4: What Are The Basic Data Types In Sql

# What Are the Basic Data Types in SQL?

To define a table in SQL, you need to specify the data type of each column.

Remember that this is the basic syntax for creating a table in SQL. Each column has its own data type.

```
CREATE TABLE table_name(
  column1 data_type column_constraint,
  column2 data_type column_constraint,
  column3 data_type column_constraint,
  ... etc
);
```

As a developer, your goal is to choose these data types as accurately as possible.

There are six popular categories of data types in SQL:

* Numeric, such as `INTEGER`, `FLOAT`, `SERIAL`, and `DECIMAL`.
* Date and time, such as `TIMESTAMP`, `DATE`, and `TIME`.
* Character and string. These include `CHAR`, `VARCHAR`, and `TEXT`.
* Unicode, including `NTEXT`, and `NVARCHAR`. These are used to make sure that text will be stored and retrieved correctly, regardless of the characters' origin.
* Binary, used to store non-textual data, like images, audio, and video files.
* And other miscellaneous data types, such as `XML` and `TABLE`.

In this lesson, we'll cover some of the most widely used ones with PostgreSQL. Data types will vary across database management systems, but they are generally pretty similar. So you'll need to check the full list in the documentation.

We'll start with numeric values.

First, we have the `INTEGER` data type:

```
units_sold INTEGER
```

In this example, we assign this data type to a `units_sold` column.

`INTEGER` types consume 4 bytes in the database and can range in value from -2,147,483,648 to 2,147,483,647. The official PostgreSQL documentation describes it as the "typical choice for integer."

We also have `SMALLINT` and `BIGINT`, which are basically the same as `INTEGER` except have a smaller and bigger range of numbers, respectively, due to how much size they are allotted in the database.

A useful feature available in PostgreSQL is to create a column using the `SERIAL` keyword. Here, an `id` column is created using `SERIAL`:

```
id SERIAL
```

While it's not a true data type, it's very helpful for creating unique identifier columns because the column will have an `INTEGER` type, will not allow `NULL` values, and automatically increment when rows are added.

For example, the first row will automatically have an `id` of `1`, the second row will have an `id` of `2`, and so on, creating a unique ID for each record.

In MySQL, the equivalent of `SERIAL` would be the `AUTO_INCREMENT` attribute, used to generate sequential integers automatically:

```
id INT AUTO_INCREMENT
```

You can see that different database management systems may have different ways of achieving exactly the same functionality in your database.

These are the most commonly used numeric data types, but sometimes, you may need to represent text or sequences of characters.

For this, you have the `VARCHAR` data type. This data type is used for a variable string length. You can set the maximum character length within parentheses:

```
name VARCHAR(50)
```

In this example, we define a `name` column, where the values can be up to 50 characters long.

This data type sets a maximum length for the strings, but if you need to store strings of any length, you can use `TEXT` instead:

```
name TEXT
```

In addition to numbers and strings, it's also common to store dates and times.

For example, if you create a table to store events, you may need to store the date of each event in a specific format. For this, you have the `DATE` data type:

```
event_date DATE
```

To store time, you can also use the `TIME` data type. For example, you may store the time when an event starts:

```
start_time TIME
```

The `TIMESTAMP` data type combines both of them. It includes both the date and time. It may also include the time zone if you write `TIMESTAMP WITH TIME ZONE`:

```
event_timestamp TIMESTAMP
```

```
event_timestamp TIMESTAMP WITH TIME ZONE
```

And finally, if you need to store a boolean value, `TRUE` or `FALSE`, you can use the `BOOLEAN` data type:

```
is_active BOOLEAN
```

Now you know some of the most common data types in SQL, but there are many more. You can check the documentation of your database management system to find more information about the data types that you can use.

---

### Lecture 5.5: How Do You Insert And View Data In A Table

# How Do You Insert and View Data in a Table?

Let's see some of the fundamental commands that you can use to insert and view data in SQL.

First of all, to view data, you need to insert it. So we'll start with insertions.

The examples that we will cover in this lesson will be based on this table of dog records:

```
CREATE TABLE dogs(
  id SERIAL,
  name VARCHAR(100),
  age INTEGER
);
```

The table will store the names and ages of various dogs.

If we assume that we are working with PostgreSQL, we can use the `SERIAL` data type for the `id`. Since `id` was created using `SERIAL`, its value will be an `INTEGER`, starting from `1`, and incremented automatically when a new record is inserted. So you will not need to pass a value for it when you insert a record.

Let's start by inserting records to our `dogs` table with the `INSERT INTO` statement. There are many ways to do this. The first one would be inserting a single row and specifying the columns of the values that will be inserted.

You write `INSERT INTO`, followed by the name of the table (in this case, `dogs`), then the columns within parentheses, then `VALUES`, and their corresponding values within parentheses.

This is an example, we're inserting a dog record with the `name` of `'Gino'`, whose `age` is `3`, remember that the `id` will be assigned automatically:

```
INSERT INTO dogs (name, age)
VALUES ('Gino', 3);
```

This is usually the safest option because you specify the columns explicitly, so the values will be assigned to those columns in order.

Notice that `'Gino'` needs to be in single quotes because it is a `VARCHAR` type.

Another alternative is to insert the record without specifying the columns, like this:

```
INSERT INTO dogs
VALUES ('Gino', 3);
```

This syntax is valid SQL, but it is error-prone.

Since values are assigned based on column order, PostgreSQL will try to insert `'Gino'` into the `id` column, which expects an integer. This results in an error such as `invalid input syntax for type integer`.

For this reason, it is safer to explicitly specify the column names when inserting data.

You can also insert multiple records in the same SQL command by separating them with a comma.

Here, we are inserting two dog records, one for `'Gino'` and another one for `'Nora'`.

```
INSERT INTO dogs (name, age)
VALUES
  ('Gino', 3),
  ('Nora', 2);
```

And just like you can insert records, you can query information from the database. In the context of databases, a query is a request for data.

In SQL, the `SELECT` statement is used for querying data from one or more tables. You can customize the query to get the exact information that you need.

If you need to query all the information from the `dogs` table, you just need to write `SELECT`, followed by an asterisk (`*`), then `FROM`, and the name of the table, `dogs`:

```
SELECT *
FROM dogs;
```

In this command, the asterisk is a wildcard character that represents "all columns."

You will get all the data of all the records in the table:

```
 id | name | age 
----+------+-----
  1 | Gino |   3
  2 | Nora |   2
```

To query specific columns, you can write the names of those columns in the command, right after `SELECT`, separated by a comma. In this example, we query the `name` and `age` columns of the `dogs` table:

```
SELECT name, age
FROM dogs;
```

The result will only include the `name` and `age` columns:

```
 name | age 
------+-----
 Gino |   3
 Nora |   2
```

Sometimes, you might need to query data based on a specific condition. For example, to get all dogs who are less than 3 years old you can use the `WHERE` keyword and the less than (`<`) comparison operator:

```
SELECT *
FROM dogs
WHERE age < 3;
```

The result will only include dogs whose age is less than 3:

```
 id | name | age 
----+------+-----
  2 | Nora |   2
```

If you are just trying to find the `age` of `'Gino'`, you can use the equals (`=`) comparison operator:

```
SELECT age
FROM dogs
WHERE name = 'Gino';
```

And here's the result:

```
 age 
-----
  3
```

These are common and simple ways to insert and view data in SQL, but there are many different options that you can choose from and some of them are more advanced. You'll learn about them in coming lessons.

---

### Lecture 5.6: What Are Primary And Foreign Keys In Sql And How Do They Work

# What Are Primary and Foreign Keys in SQL, and How Do They Work?

In SQL, primary keys and foreign keys are used to establish relationships between tables.

Let's start with primary keys.

A primary key is a column or set of columns that uniquely identifies each record (row) in a table. This constraint ensures that no records in the table will have the same value for the primary key.

This is why a table can only have one primary key.

Values in the primary key column can't be `NULL` either, so they will always have a valid value.

In PostgreSQL, to make a column the primary key of your table, you just need to add `PRIMARY KEY` after the data type:

```
column_name data_type PRIMARY KEY
```

This is an example of a `students` table:

```
CREATE TABLE students (
  student_id SERIAL PRIMARY KEY,
  name VARCHAR(100)
);
```

Each student will have its own `student_id`, and this ID will be the primary key of the table. The `SERIAL` type is useful here because it ensures the `student_id` will always have a unique value.

A composite primary key is for when a table doesn't have a single unique column to identify the row. In this case, you can use a combination of two or more columns as the primary key that, together, are unique.

To do this, denote which columns are the composite primary key when you create the table like this:

```
CREATE TABLE table_name (
  column1 data_type column_constraint,
  column2 data_type column_constraint,
  column3 data_type column_constraint,
  ...
  PRIMARY KEY (column1, column2)
);
```

Imagine you have a table with `student_id` and `course_id` columns that tells you what students are enrolled in various classes.

Each student will be enrolled in several classes, and each class will have several students enrolled in it. So neither column is unique - but you will never have the same student enrolled in the same class more than once. So you can use the combination of the two columns as the primary key:

```
CREATE TABLE course_enrollments (
  student_id INT,
  course_id INT,
  ...
  PRIMARY KEY (student_id, course_id),
);
```

Primary keys are essential for ensuring data uniqueness and integrity, for optimizing data retrieval, and for establishing relationships with other tables in a relational database.

That takes us to the next type of key that we will cover in this lesson: foreign keys.

A foreign key is a column (or set of columns) in a table that references the primary key of another table. A table can have multiple foreign keys.

In this example, we have two tables, `customers`, and `orders`:

```
CREATE TABLE customers (
  customer_id SERIAL PRIMARY KEY,
  first_name VARCHAR(100) NOT NULL,
  ...
);

CREATE TABLE orders (
  order_id SERIAL PRIMARY KEY,
  customer_id INTEGER,
  ...
  FOREIGN KEY (customer_id) REFERENCES customers(customer_id)
);
```

The primary key of the `customers` table is `customer_id` and the primary key of the `orders` table is `order_id`.

But notice that there is also a `customer_id` column in the `orders` table.

Why are we storing customer information in the `orders` table?

We do this to create a relationship between the `customers` and `orders` tables. Each order will store the ID of the customer who submitted it.

To create the relationship between the tables, we will make the `customer_id` column in the `orders` table a foreign key that references the `customer_id` column in the `customers` table:

```
FOREIGN KEY (customer_id) REFERENCES customers(customer_id)
```

Values in a foreign key column must either match the primary key values in the referenced table or be `NULL` (if the foreign key allows `NULL`s).

Why is this helpful?

By making sure that these columns in both tables match exactly, foreign and primary keys prevent the creation of "orphaned" records, records that refer to a non-existent record in another table.

Primary and foreign keys are fundamental for relational databases. They power the "relational" aspect of these databases, allowing you to model real-world data in an accurate way.

---

### Lecture 5.7: What Are The Different Types Of Relationships In A Relational Database

# What Are the Different Types of Relationships in a Relational Database?

Like you learned in previous lessons, relational databases store data in tables, which are made of rows and columns.

The "relational" aspect of "relational databases" comes from the fact that records in different tables can have different types of relationships.

There are five main types of relations:

* one-to-one
* one-to-many
* many-to-one
* many-to-many
* And self-referencing relationships (also known as recursive relationships).

Two tables have a **one-to-one** relationship when each record in the first table can be associated with at most one record in the second table, and vice versa.

For example, let's say a company only assigns one vehicle per employee.

In that case, the database could have an `employees` table and a `vehicles` table, where each employee record corresponds to one, and only one, vehicle record in the database.

In contrast, **one-to-many** relationships occur when one record in a table can be related to one or more records in another table.

For example, if we have a `customers` table and an `orders` table, each customer could be related to one or more orders but each order can only be related to one customer.

This is the same as the **many-to-one** relation, but from the opposite perspective. One or more orders can be related to one customer.

**Many-to-many** relationships occur when a record in a table can be related to multiple records in another table and vice versa.

For example, let's analyze a database for a library. For simplicity purposes, let's assume that this database only has two tables: `books` and `authors`.

An author can write multiple books, and a single book can be written by multiple authors.

Implementing this type of relationship is a little bit more complex because the relational model at its core doesn't support many-to-many relationships directly.

To handle this, you would usually create an intermediate table, also known as a junction table.

This table solves these initial limitations by transforming the many-to-many relationship into two one-to-many relationships.

It creates a one-to-many relationship between the first table and the junction table and a one-to-many relationship between the second table and the junction table.

The name of the junction table is usually a combination of the entities. In the context of our example of `books` and `authors`, you may call it `books_authors`.

In the junction table itself, you would associate the authors and their books by creating two columns: a column for the author's id (`author_id`) and another column for the book's id (`book_id`).

These would be foreign keys referencing their corresponding primary keys in the `authors` and `books` tables, respectively.

With this junction table, you'll be able to query all the authors of a given book or all books written by a given author.

Using a junction table makes it easier to query the data, prevents redundancy, and simplifies the database schema. They are very helpful for implementing many-to-many relationships.

And finally, we find **self-referencing** relationships, which occur when the records of a table can be related to other records on the same table. This is also known as a recursive relationship.

Understanding these relationships is essential for designing and modeling complex and efficient relational databases.

---

### Lecture 5.8: What Are The Different Ways To Join Tables

# What Are the Different Ways to Join Tables?

Even though relational databases organize data into separate tables, SQL's `JOIN` operations allow you to combine related information from tables to query data.

There are several variants of the `JOIN` operation, including:

* `INNER JOIN`
* `FULL OUTER JOIN`
* `LEFT OUTER JOIN`
* `RIGHT OUTER JOIN`
* `SELF JOIN`
* `CROSS JOIN`

Let's start with `INNER JOIN`.

An `INNER JOIN` filters the result to include only rows where the values in the joining columns that you specify are equal in both tables. Basically, it gives you the intersection of the data.

To illustrate this, let's say that we have two tables.

The first is this `products` table with multiple products. It includes their ID's, names, category, price, and origin.

```
| product_id | product_name     | category    | price (USD) | origin        |
| ---------- | ---------------- | ----------- | ----------- | ------------- |
| 1          | Ice Cream        | Food        | 2.50        | India         |
| 2          | Pizza Margherita | Food        | 12.00       | Italy         |
| 3          | Sushi            | Food        | 18.75       | Japan         |
| 4          | T-Shirt          | Clothing    | 25.00       | USA           |
| 5          | Jeans            | Clothing    | 60.00       | Argentina     |
| 6          | Coffee           | Beverages   | 35.00       | France        |
| 7          | Juice            | Beverages   | 5.00        | Colombia      |
```

And second, we have a `sales` table, with the sale ID, product ID, quantity, and sale date.

```
| sale_id | product_id | quantity | sale_date  |
| ------- | ---------- | -------- | ---------- |
| 101     | 1          | 2        | 2025-07-18 |
| 102     | 2          | 3        | 2025-02-13 |
| 103     | 6          | 10       | 2025-06-08 |
| 104     | 5          | 8        | 2025-01-10 |
| 105     | 2          | 1        | 2025-05-15 |
```

We can perform an `INNER JOIN` based on the `product_id` like this:

```
SELECT *
FROM products
INNER JOIN sales
  ON products.product_id = sales.product_id;
```

This will only get the rows that have the same `product_id` in both tables. So if a product is not in the sales table or in products table, it will not be included.

This is the result:

```
product_id | product_name     | category  | price | origin    | sale_id | product_id | quantity | sale_date
---------- | ---------------- | --------- |-------|-----------|---------|------------|----------|------------
     1     | Ice Cream        | Food      |  2.50 | India     |     101 |          1 |        2 | 2025-07-18
     2     | Pizza Margherita | Food      | 12.00 | Italy     |     102 |          2 |        3 | 2025-02-13
     2     | Pizza Margherita | Food      | 12.00 | Italy     |     105 |          2 |        1 | 2025-05-15
     5     | Jeans            | Clothing  | 60.00 | Argentina |     104 |          5 |        8 | 2025-01-10
     6     | Coffee           | Beverages | 35.00 | France    |     103 |          6 |       10 | 2025-06-08
```

We only see the rows of the products that have been sold. For example, `'Pizza Margherita'` is in the `sales` table, with a `product_id` of `2`, so we get that product in the result.

However, `'T-Shirts'` with a `product_id` of `4` were not sold, so this product is not in the `sales` table. They are not in both tables, so they are not included in the result.

Joining tables does exactly what it sounds like. It joins two or more tables into one, which is why we see all the columns from both tables, including `product_id` twice.

A `FULL OUTER JOIN` returns all rows from both tables.

If a match is found in the specified columns, the data is combined and you get all columns for each matching record.

If there's no match in the specified columns, in either one of the tables, the missing columns are filled with `NULL` values.

Let's perform a `FULL OUTER JOIN` in our example, based on the `product_id` column. This column will determine if there is a match or not.

```
SELECT *
FROM products
FULL OUTER JOIN sales
  ON products.product_id = sales.product_id;
```

This is the result:

```
product_id | product_name     | category  | price | origin    | sale_id | product_id | quantity | sale_date
---------- | ---------------- | --------- |-------|-----------|---------|------------|----------|------------
         1 | Ice Cream        | Food      |  2.50 | India     |     101 |          1 |        2 | 2025-07-18
         2 | Pizza Margherita | Food      | 12.00 | Italy     |     102 |          2 |        3 | 2025-02-13
         3 | Sushi            | Food      | 18.75 | Japan     |         |            |          |
         4 | T-Shirt          | Clothing  | 25.00 | USA       |         |            |          |
         5 | Jeans            | Clothing  | 60.00 | Argentina |     104 |          5 |        8 | 2025-01-10
         6 | Coffee           | Beverages | 35.00 | France    |     103 |          6 |       10 | 2025-06-08
         7 | Juice            | Beverages |  5.00 | Colombia  |         |            |          |
         2 | Pizza Margherita | Food      | 12.00 | Italy     |     105 |          2 |        1 | 2025-05-15
```

Notice how `'Pizza Margherita'` has all the data, including columns from the `sales` table because there was a match.

But `'T-Shirt'` has empty (`NULL`) columns because no match was found in the `sales` table (this product was not sold).

A `LEFT OUTER JOIN` is used to get all the records from the left table and the matching information from the right table for each row of the left table.

If no match is found, the columns from the right table are filled in with `NULL` values.

Let's perform a `LEFT OUTER JOIN` in our example.

```
SELECT *
FROM products
LEFT JOIN sales
  ON products.product_id = sales.product_id;
```

This is the result:

```
product_id | product_name     | category  | price | origin    | sale_id | product_id | quantity | sale_date
---------- | ---------------- | --------- |-------|-----------|---------|------------|----------|------------
         1 | Ice Cream        | Food      |  2.50 | India     |     101 |          1 |        2 | 2025-07-18
         2 | Pizza Margherita | Food      | 12.00 | Italy     |     102 |          2 |        3 | 2025-02-13
         3 | Sushi            | Food      | 18.75 | Japan     |         |            |          |
         4 | T-Shirt          | Clothing  | 25.00 | USA       |         |            |          |
         5 | Jeans            | Clothing  | 60.00 | Argentina |     104 |          5 |        8 | 2025-01-10
         6 | Coffee           | Beverages | 35.00 | France    |     103 |          6 |       10 | 2025-06-08
         7 | Juice            | Beverages |  5.00 | Colombia  |         |            |          |
         2 | Pizza Margherita | Food      | 12.00 | Italy     |     105 |          2 |        1 | 2025-05-15
```

In this case, it's the same as the `FULL OUTER JOIN` because it includes all rows from the first table, `products`.

A `RIGHT OUTER JOIN` is very similar, but now we get all the records from the right table and the matching information from the left table for each row of the right table.

If there's no match, the columns from the left table are filled in with `NULL` values.

Let's perform a `RIGHT OUTER JOIN` in our example.

```
SELECT *
FROM products
RIGHT JOIN sales
  ON products.product_id = sales.product_id;
```

Here is the result:

```
product_id | product_name     | category  | price | origin    | sale_id | product_id | quantity | sale_date
---------- | ---------------- | --------- |-------|-----------|---------|------------|----------|------------
         1 | Ice Cream        | Food      |  2.50 | India     |     101 |          1 |        2 | 2025-07-18
         2 | Pizza Margherita | Food      | 12.00 | Italy     |     102 |          2 |        3 | 2025-02-13
         6 | Coffee           | Beverages | 35.00 | France    |     103 |          6 |       10 | 2025-06-08
         5 | Jeans            | Clothing  | 60.00 | Argentina |     104 |          5 |        8 | 2025-01-10
         2 | Pizza Margherita | Food      | 12.00 | Italy     |     105 |          2 |        1 | 2025-05-15
```

You'll notice that it has fewer rows. This is because it takes all the records from the right table (`sales` in this case), and this table has fewer rows than the `products` table.

If it finds a match in the `products` table, it fills those columns with the data. But if there's no match, the columns are filled with `NULL`.

In this case, every product that has been sold has a record in the `products` table, so the data is complete.

These are the most commonly-used `JOIN` operations, but there are two additional ones that you should know about.

A `SELF JOIN` allows you to join the table with itself. You can think of it as joining two copies of the same table. This is helpful for comparing different rows within the same table.

A `CROSS JOIN`, also known as a Cartesian Join, joins every row from the first table with every row of the second table. Therefore, it generates all possible row combinations. This operation doesn't need any conditions to join the tables.

These `JOIN` operations are fundamental for working with SQL. By choosing the right one, you can query the data you need as efficiently as possible.

---

### Section Summary: Relational Databases

# Relational Databases Review

Terminal, Shell, and Command Line Basics
----------------------------------------

* **Command line**: A text interface where users type commands.
* **Terminal**: The application that provides access to the command line.
* **Terminal emulator**: Adds extra features to a terminal.
* **Shell**: Interprets the commands entered into the terminal (e.g., Bash).
* **PowerShell / Command Prompt / Microsoft Terminal**: Options for accessing the command line on Windows.
* **Terminal (macOS)**: Built-in option on macOS, with third-party alternatives like iTerm or Ghostty.
* **Terminal (Linux)**: Options vary by distribution, with many third-party emulators like kitty.
* **Terminology**: Though "terminal," "shell," and "command line" are often used interchangeably, they have specific meanings.

Command Line Shortcuts
----------------------

* **Up/Down arrows**: Cycle through previous/next commands in history.
* **Tab**: Autocomplete commands.
* **`Control+L`** (Linux/macOS) or typing `cls` (Windows): Clear the terminal screen.
* **`Control+C`**: Interrupt a running command (also used for copying in PowerShell if text is selected).
* **`Control+Z`** (Linux/macOS only): Suspend a task to the background; use `fg` to resume it.
* **`!!`**: Instantly rerun the last executed command.

Bash Basics
-----------

* **Bash** (Bourne Again Shell): Widely used Unix-like shell.  
  Key commands:

  + **`pwd`**: Show the current directory.
  + **`cd`**: Change directories.
    - **`..`** refers to the parent directory (one level up).
    - **`.`** refers to the current directory.
  + **`ls`**: List files and folders.
    - **`-a`**: Show all files, including hidden files.
    - **`-l`**: Show detailed information about files.
  + **`less`**: View file contents one page at a time with navigation options, including scrolling backward and searching.
  + **`more`**: Display file contents one screen at a time, with limited backward scrolling and basic navigation.
  + **`cat`**: Show the entire file content at once without scrolling or navigation, useful for smaller files.
  + **`mkdir`**: Create a new directory.
  + **`rmdir`**: Remove an empty directory.
  + **`touch`**: Create a new file.
  + **`mv`**: Move or rename files.
    - Rename: `mv oldname.txt newname.txt`
    - Move: `mv filename.txt /path/to/target/`
  + **`cp`**: Copy files.
    - **`-r`**: Recursively copy directories and their contents.
  + **`rm`**: Delete files.
    - **`-r`**: Recursively delete directories and their contents.
  + **`echo`**: Display a line of text or a variable's value.
    - Use `>` to overwrite the existing content in a file. (e.g., `echo "text" > file.txt`)
    - Use `>>` to append output to a file **without overwriting existing content** (e.g., `echo "text" >> file.txt`).
  + **`exit`**: Exit the terminal session.
  + **`clear`**: Clear the terminal screen.
  + **`find`**: Search for files and directories.
    - **`-name`**: Search for files by name pattern (e.g., `find . -name "*.txt"`).
  + Use **`man`** followed by a command (e.g., `man ls`) to access detailed manual/help pages.

Command Options and Flags
-------------------------

* **Options** or **flags**: modify a command's behavior and are usually prefixed with hyphens:
  + **Long form (two hyphens)**:
    - Example: `--help`, `--version`
    - Values are attached using an equals sign, e.g., `--width=50`.
  + **Short form (one hyphen)**:
    - Example: `-a`, `-l`
    - Values are passed with a space, e.g., `-w 50`.
    - Multiple short options can be chained together, e.g., `ls -alh`.
* **`--help`**: You can always use a command with this flag to understand the available options for any command.

Introduction to Relational Databases
------------------------------------

* **Relational Databases**: Organize data into related tables made of rows and columns. Each row represents a record, and each column represents an attribute of the data.
* **Advantages of Relational Databases**: Scalable, widely applicable across domains (e.g., healthcare, business, gaming), and structured to maintain reliable data.
* **Common Use Cases**: Web development, inventory systems, e-commerce, healthcare, and enterprise applications.

Key Concepts
------------

* **Schema**: A relational database requires a schema that defines its structure—tables, columns, data types, constraints, and relationships.
* **Primary Keys**: Unique identifiers for each row in a table. They are essential for data integrity and are used to relate records between tables via foreign keys.
* **Foreign Keys**: References to primary keys in another table, used to link related data across tables.
* **Relationships**: By connecting tables through primary and foreign keys, you can structure normalized data and perform meaningful queries.
* **Entity Relationship Diagrams (ERDs)**: Visualize how entities (tables) relate to each other in a database schema.
* **Data Integrity**: Enforced using keys and data types. Ensures consistency and accuracy of stored data.

SQL Basics
----------

* **Queries**: Requests to retrieve specific data from the database.

```
SELECT * FROM dogs WHERE age < 3;
```

* **WHERE clause**: Filter results based on conditions. Use comparison operators like `<`, `=`, `>`, etc.
* **Select with ORDER BY**: Retrieve and sort results based on a column.

```
SELECT columns FROM table_name ORDER BY column_name;
```

Table Operations
----------------

* **`CREATE TABLE` Statement**: This statement is used to create a new table in a database.

```
CREATE TABLE first_table();
```

* **`ALTER TABLE ADD COLUMN` Statement**: This statement is used to add a column to an existing table.

```
ALTER TABLE table_name ADD COLUMN column_name DATATYPE;
```

* **`ALTER TABLE DROP COLUMN` Statement**: This statement is used to drop a column from an existing table.

```
ALTER TABLE table_name DROP COLUMN column_name;
```

* **`ALTER TABLE RENAME COLUMN` Statement**: This statement is used to rename a column in a table.

```
ALTER TABLE table_name RENAME COLUMN column_name TO new_name;
```

* **`DROP TABLE` Statement**: This statement is used to drop an entire table from the database.

```
DROP TABLE table_name;
```

* **`ALTER DATABASE RENAME` Statement**: This statement is used to rename a database.

```
ALTER DATABASE database_name RENAME TO new_database_name;
```

* **`DROP DATABASE` Statement**: This statement is used to drop an entire database.

```
DROP DATABASE database_name;
```

Constraints & Data Integrity
----------------------------

* **`ALTER TABLE ADD COLUMN` with Constraint**: This statement is used to add a column with a constraint to an existing table.

```
ALTER TABLE table_name ADD COLUMN column_name DATATYPE CONSTRAINT;
```

* **`NOT NULL` Constraint**: This constraint ensures that a column cannot have NULL values.

```
column_name VARCHAR(50) NOT NULL
```

* **`ALTER TABLE ADD PRIMARY KEY` Statement**: This statement is used to add a primary key constraint to a table.

```
ALTER TABLE table_name ADD PRIMARY KEY(column_name);
```

* **`ALTER TABLE DROP CONSTRAINT` Statement**: This statement is used to drop a constraint from a table.

```
ALTER TABLE table_name DROP CONSTRAINT constraint_name;
```

* **`ALTER TABLE ADD COLUMN` with Foreign Key**: This statement is used to add a foreign key column that references another table.

```
ALTER TABLE table_name ADD COLUMN column_name DATATYPE REFERENCES referenced_table_name(referenced_column_name);
```

* **`ALTER TABLE ADD UNIQUE` Statement**: This statement is used to add a UNIQUE constraint to a column.

```
ALTER TABLE table_name ADD UNIQUE(column_name);
```

* **`ALTER TABLE ALTER COLUMN SET NOT NULL` Statement**: This statement is used to set a NOT NULL constraint on an existing column.

```
ALTER TABLE table_name ALTER COLUMN column_name SET NOT NULL;
```

* **`INSERT` Statement with NULL Values**: This statement demonstrates how to insert NULL values into a table.

```
INSERT INTO table_name(column_a) VALUES(NULL);
-- or
INSERT INTO table_name(column_b) VALUES('value'); -- if column_a allows nulls
```

* **Composite Primary Key**: This constraint defines a primary key that consists of multiple columns.

```
CREATE TABLE course_enrollments (
    student_id INT,
    course_id INT,
    PRIMARY KEY (student_id, course_id)
);
```

Data Manipulation (CRUD)
------------------------

* **`INSERT` Statement**: This statement is used to insert a single row into a table.

```
INSERT INTO table_name(column_1, column_2) VALUES(value1, value2);
```

* **`INSERT` Statement with Omitted Columns**: This statement shows how to insert values without explicitly listing the column names, relying on the default column order in the table.

```
INSERT INTO dogs VALUES ('Gino', 3);
```

* **`INSERT` Statement with Multiple Rows**: This statement is used to insert multiple rows into a table in a single operation.

```
INSERT INTO dogs (name, age) VALUES 
('Gino', 3),
('Nora', 2);
```

* **`UPDATE` Statement**: This statement is used to update existing data in a table based on a condition.

```
UPDATE table_name SET column_name=new_value WHERE condition;
```

* **`DELETE` Statement**: This statement is used to delete rows from a table based on a condition.

```
DELETE FROM table_name WHERE condition;
```

Data Types
----------

* **`NUMERIC` Data Type**: This data type is used to store precise decimal numbers with a specified precision and scale.

```
price NUMERIC(10, 2)
```

* **`TEXT` Data Type**: This data type is used to store variable-length character strings with no specific length limit.

```
column_name TEXT
```

* **`INTEGER` Data Type**: This data type is used to store whole numbers without decimal places.

```
units_sold INTEGER
```

* **`SMALLINT` and `BIGINT` Data Types**: These are variants of INTEGER with smaller and larger ranges respectively.
* **`SERIAL` Data Type**: This data type is used to create auto-incrementing integer columns in PostgreSQL.

```
id SERIAL
```

* **`AUTO_INCREMENT` Attribute**: This attribute is used in MySQL to create auto-incrementing integer columns.

```
id INT AUTO_INCREMENT
```

* **`VARCHAR` Data Type**: This data type is used to store variable-length character strings with a specified maximum length.

```
name VARCHAR(50)
```

* **`DATE` Data Type**: This data type is used to store date values (year, month, day).

```
event_date DATE
```

* **`TIME` Data Type**: This data type is used to store time values (hour, minute, second).

```
start_time TIME
```

* **`TIMESTAMP` Data Type**: This data type is used to store date and time values, optionally with time zone information.

```
event_timestamp TIMESTAMP
event_timestamp TIMESTAMP WITH TIME ZONE
```

* **`BOOLEAN` Data Type**: This data type is used to store true/false values.

```
is_active BOOLEAN
```

Database Relationships
----------------------

* **Types of Relationships**: These are the different ways tables can be related to each other in a relational database.

  + One-to-one
  + One-to-many
  + Many-to-one
  + Many-to-many
  + Self-referencing (recursive)
* **One-to-One Relationship**: This relationship type means that each record in one table corresponds to exactly one record in another table.

```
One employee is assigned exactly one vehicle.
Tables: employees, vehicles
```

* **One-to-Many Relationship**: This relationship type means that one record in a table can be associated with multiple records in another table.

```
One customer can have many orders.
Tables: customers → orders
```

* **Many-to-Many Relationship via Junction Table**: This relationship type is implemented using a junction table that contains foreign keys from both related tables.

```
CREATE TABLE books_authors (
    author_id INT REFERENCES authors(id),
    book_id INT REFERENCES books(id)
);
```

* **Self-Referencing Relationships**: This relationship type occurs when a table references itself, creating a hierarchical structure.

```
An employee table where each employee may report to another employee.
```

Advanced SQL (Joins)
--------------------

* **`INNER JOIN` Statement**: This join returns only the rows that have matching values in both tables.

```
SELECT *
FROM products
INNER JOIN sales ON products.product_id = sales.product_id;
```

* **`FULL OUTER JOIN` Statement**: This join returns all rows from both tables, including unmatched rows from either table.

```
SELECT *
FROM products
FULL OUTER JOIN sales ON products.product_id = sales.product_id;
```

* **`LEFT OUTER JOIN` Statement**: This join returns all rows from the left table and matching rows from the right table.

```
SELECT *
FROM products
LEFT JOIN sales ON products.product_id = sales.product_id;
```

* **`RIGHT OUTER JOIN` Statement**: This join returns all rows from the right table and matching rows from the left table.

```
SELECT *
FROM products
RIGHT JOIN sales ON products.product_id = sales.product_id;
```

* **`SELF JOIN` Statement**: This join is used to join a table with itself to compare rows within the same table.

```
SELECT A.column_name, B.column_name
FROM table_name A
JOIN table_name B ON A.related_column = B.related_column;
```

* **`CROSS JOIN` Statement**: This join returns the Cartesian product of two tables, combining every row from the first table with every row from the second table.

```
SELECT *
FROM table1
CROSS JOIN table2;
```

PostgreSQL Specific Commands
----------------------------

* **`psql` Login Command**: This command is used to log in to PostgreSQL with specific username and database.

```
psql --username=freecodecamp --dbname=postgres
```

* **`\l` Command**: This command lists all databases in the PostgreSQL instance.

```
\l
```

* **`CREATE DATABASE` and `\c` Commands**: These commands are used to create a new database and connect to it.

```
CREATE DATABASE database_name;
\c database_name
```

* **`\d` Command**: This command lists all tables in the current database.

```
\d
```

* **`\d table_name` Command**: This command displays the schema/structure of a specific table.

```
\d table_name
```

* **`\q` Command**: This command exits the PostgreSQL client.

```
\q
```

Relational vs Non-Relational
----------------------------

* **Non-Relational (NoSQL) Databases**: Store unstructured or semi-structured data. Do not require a rigid schema and are more flexible for evolving data models.
* **Choosing Between Relational and Non-Relational**: Depends on the nature of your data and application requirements.
* **Relational vs Non-Relational**: Choose relational for structured data and consistency; NoSQL for flexibility and fast-changing data.

Popular RDBMS Systems
---------------------

* **MySQL**: Open-source, reliable, widely used in web development, supported by a large community.
* **PostgreSQL**: Open-source, advanced, extensible. Supports custom data types and server-side programming.
* **SQLite**: Lightweight, file-based, serverless. Ideal for small applications.
* **Microsoft SQL Server**: Proprietary, enterprise-grade database.
* **Oracle Database**: Commercial RDBMS known for large-scale performance and scalability.

Best Practices
--------------

* **Naming Convention**: Use `snake_case` (e.g., `delivery_orders`) for table and column names.

Bash Scripting Basics
---------------------

* **Bash scripting**: Writing a sequence of Bash commands in a file, which you can then execute with Bash to run the contents of the file.
* **Shebang**: The commented line at the beginning of a script (e.g., `#!/bin/bash`) that indicates what interpreter should be used for the script.

  ```
  #!/bin/bash
  ```
* **Variable assignment**: Instantiate variables using the syntax `variable_name=value`.

  ```
  servers=("prod" "dev")
  ```
* **Variable creation rules**: Create variables with `VARIABLE_NAME=VALUE` syntax. No spaces are allowed around the equal sign (`=`). Use double quotes if the value contains spaces.

  ```
  NAME=John
  MESSAGE="Hello World"
  COUNT=5
  TEXT="The next number is, "
  ```
* **Variable usage**: Access variable values by placing `$` in front of the variable name.

  ```
  echo $NAME
  echo "The message is: $MESSAGE"
  ```
* **Variable interpolation**: Use `$variable_name` to access the value of a variable within strings and commands.

  ```
  TEXT="The next number is, "
  NUMBER=42
  echo $TEXT B:$NUMBER
  echo $TEXT I:$NUMBER

  echo "Pulling $server"
  rsync --archive --verbose $server:/etc/nginx/conf.d/server.conf configs/$server.conf
  ```
* **Variable scope**: Shell scripts run from top to bottom, so variables can only be used below where they are created.

  ```
  NAME="Alice"
  echo $NAME
  ```
* **User input**: Use `read` to accept input from users and store it in a variable.

  ```
  read USERNAME
  echo "Hello $USERNAME"
  ```
* **Comments**: Add comments to your scripts using `#` followed by your comment text.

  + Single-line comments start with `#` and continue to the end of the line
  + Comments are ignored by the shell and don't affect script execution

  ```
  # This is a single-line comment
  NAME="John"  # Comment at end of line
  ```
* **Multi-line comments**: Comment out blocks of code using colon and quotes.

  ```
  : '
  This is a multi-line comment
  Everything between the quotes is ignored
  Useful for debugging or documentation
  '
  ```
* **Built-in commands and help**:

  + Use `help` to see a list of built-in bash commands
  + Use `help <command>` to get information about specific built-in commands
  + Some commands (like `if`) are built-ins and don't have man pages
  + Built-in commands are executed directly by the shell rather than as external programs
  + Use `help function` to see information about creating functions

  ```
  help
  help if
  help function
  ```
* **Finding command locations**: Use `which` to locate where executables are installed.

  + Shows the full path to executable files
  + Useful for finding interpreter locations (like bash)
  + Helps verify which version of a command will be executed

  ```
  which bash
  which python
  which ls
  ```
* **Manual pages**: Use `man` to access detailed documentation for commands.

  + Provides comprehensive information about command usage
  + Shows all available options and examples
  + Use arrow keys to navigate, 'q' to quit
  + Not all commands have manual pages (built-ins use `help` instead)

  ```
  man echo
  man ls
  man bash
  ```
* **Help flags**: Many commands support `--help` for quick help information.

  + Alternative to manual pages for quick reference
  + Shows command syntax and common options
  + Not all commands support this flag (some may show error)

  ```
  ls --help
  chmod --help
  mv --help
  ```
* **Echo command options**: The `echo` command supports various options:

  + `-e` option enables interpretation of backslash escapes
  + `\n` creates a new line
  + Empty lines are only printed when values are enclosed in quotes
  + Useful for creating formatted output and program titles

  ```
  echo -e "Line 1\nLine 2"
  echo ""
  echo -e "\n~~ Program Title ~~\n"
  echo "Line 1\nLine 2"
  ```
* **Script arguments**: Programs can accept arguments that are accessible using `$` variables.

  + `$*` prints all arguments passed to the script
  + `$@` prints all arguments passed to the script as separate quoted strings
  + `$<number>` accesses specific arguments by position (e.g., `$1`, `$2`, `$3`)

  ```
  echo $*
  echo $@
  echo $1
  echo $2
  ```

Double Bracket Expressions `[[ ]]`
----------------------------------

* **Double bracket syntax**: Use `[[ ]]` for conditional testing and pattern matching.

  + Must have spaces inside the brackets and around operators
  + Returns exit status 0 (true) or 1 (false) based on the test result

  ```
  [[ $variable == "value" ]]
  [[ $number -gt 10 ]]
  [[ -f filename.txt ]]
  ```
* **String comparison operators**: Compare strings using various operators within `[[ ]]`.

  + `==` (equal): Tests if two strings are identical
  + `!=` (not equal): Tests if two strings are different
  + `<` (lexicographically less): String comparison in alphabetical order
  + `>` (lexicographically greater): String comparison in alphabetical order

  ```
  [[ "apple" == "apple" ]]
  [[ "apple" != "orange" ]]
  [[ "apple" < "banana" ]]
  [[ "zebra" > "apple" ]]
  ```
* **Numeric comparison operators**: Compare numbers using specific numeric operators.

  + `-eq` (equal): Numeric equality comparison
  + `-ne` (not equal): Numeric inequality comparison
  + `-lt` (less than): Numeric less than comparison
  + `-le` (less than or equal): Numeric less than or equal comparison
  + `-gt` (greater than): Numeric greater than comparison
  + `-ge` (greater than or equal): Numeric greater than or equal comparison

  ```
  [[ $number -eq 5 ]]
  [[ $count -ne 0 ]]
  [[ $age -ge 18 ]]
  [[ $score -lt 100 ]]
  ```
* **Logical operators**: Combine multiple conditions using logical operators.

  + `&&` (and): Both conditions must be true
  + `||` (or): At least one condition must be true
  + `!` (not): Negates the condition (makes true false, false true)

  ```
  [[ $age -ge 18 && $age -le 65 ]]
  [[ $name == "John" || $name == "Jane" ]]
  [[ ! -f missing_file.txt ]]
  ```
* **File test operators**: Test file properties and existence.

  + `-e file`: True if file exists
  + `-f file`: True if file exists and is a regular file
  + `-d file`: True if file exists and is a directory
  + `-r file`: True if file exists and is readable
  + `-w file`: True if file exists and is writable
  + `-x file`: True if file exists and is executable
  + `-s file`: True if file exists and has size greater than zero

  ```
  [[ -e /path/to/file ]]
  [[ -f script.sh ]]
  [[ -d /home/user ]]
  [[ -x program ]]
  ```
* **Pattern matching with `=~`**: Use regular expressions for advanced pattern matching.

  + `=~` operator enables regex pattern matching
  + Pattern should not be quoted when using regex metacharacters
  + Supports full regular expression syntax
  + Case-sensitive by default

  ```
  [[ "hello123" =~ [0-9]+ ]]
  [[ "email@domain.com" =~ ^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$ ]]
  [[ "filename.txt" =~ \.txt$ ]]
  ```
* **Variable existence testing**: Check if variables are set or empty.

  + Test if variable is empty: `[[ ! $variable ]]`

  ```
  [[ ! $undefined_var ]]
  ```

Double Parentheses Expressions `(( ))`
--------------------------------------

* **Arithmetic evaluation**: Use `(( ))` for mathematical calculations and numeric comparisons.

  + Evaluates arithmetic expressions using C-style syntax
  + Variables don't need `$` prefix inside double parentheses
  + Returns exit status 0 if result is non-zero, 1 if result is zero
  + Supports all standard arithmetic operators

  ```
  (( result = 10 + 5 ))
  (( count++ ))
  (( total += value ))
  ```
* **Arithmetic operators**: Mathematical operators available in `(( ))`.

  + `+` (addition): Add two numbers
  + `-` (subtraction): Subtract second number from first
  + `*` (multiplication): Multiply two numbers
  + `/` (division): Divide first number by second (integer division)
  + `%` (modulo): Remainder after division
  + `**` (exponentiation): Raise first number to power of second

  ```
  (( sum = a + b ))
  (( diff = x - y ))
  (( product = width * height ))
  (( remainder = num % 10 ))
  (( power = base ** exponent ))
  ```
* **Assignment operators**: Modify variables using arithmetic assignment operators.

  + `=` (assignment): Assign value to variable
  + `+=` (add and assign): Add value to variable
  + `-=` (subtract and assign): Subtract value from variable
  + `*=` (multiply and assign): Multiply variable by value
  + `/=` (divide and assign): Divide variable by value
  + `%=` (modulo and assign): Set variable to remainder

  ```
  (( counter = 0 ))
  (( counter += 5 ))
  (( total -= cost ))
  (( area *= 2 ))
  (( value /= 3 ))
  ```
* **Increment and decrement operators**: Modify variables by one.

  + `++variable` (pre-increment): Increment before use
  + `variable++` (post-increment): Increment after use
  + `--variable` (pre-decrement): Decrement before use
  + `variable--` (post-decrement): Decrement after use

  ```
  (( ++counter ))
  (( index++ ))
  (( --remaining ))
  (( attempts-- ))
  ```
* **Comparison operators**: Compare numbers using arithmetic comparison.

  + `==` (equal): Numbers are equal
  + `!=` (not equal): Numbers are not equal
  + `<` (less than): First number is less than second
  + `<=` (less than or equal): First number is less than or equal to second
  + `>` (greater than): First number is greater than second
  + `>=` (greater than or equal): First number is greater than or equal to second

  ```
  (( age >= 18 ))
  (( score < 100 ))
  (( count == 0 ))
  (( temperature > freezing ))
  ```
* **Logical operators**: Combine arithmetic conditions.

  + `&&` (and): Both conditions must be true
  + `||` (or): At least one condition must be true
  + `!` (not): Negates the condition

  ```
  (( age >= 18 && age <= 65 ))
  (( score >= 90 || extra_credit > 0 ))
  (( !(count == 0) ))
  ```
* **Bitwise operators**: Perform bit-level operations on integers.

  + `&` (bitwise AND): AND operation on each bit
  + `|` (bitwise OR): OR operation on each bit
  + `^` (bitwise XOR): XOR operation on each bit
  + `~` (bitwise NOT): Invert all bits
  + `<<` (left shift): Shift bits to the left
  + `>>` (right shift): Shift bits to the right

  ```
  (( result = a & b ))
  (( flags |= new_flag ))
  (( shifted = value << 2 ))
  ```
* **Conditional (ternary) operator**: Use `condition ? true_value : false_value` syntax.

  + Provides a concise way to assign values based on conditions
  + Similar to the ternary operator in C-style languages
  + Evaluates condition and returns one of two values

  ```
  (( result = (score >= 60) ? 1 : 0 ))
  (( max = (a > b) ? a : b ))
  (( sign = (num >= 0) ? 1 : -1 ))
  ```
* **Command substitution with arithmetic**: Use `$(( ))` to capture arithmetic results.

  + Returns the result of the arithmetic expression as a string
  + Can be used in assignments or command arguments
  + Useful for calculations that need to be used elsewhere

  ```
  result=$(( 10 + 5 ))
  echo "The answer is $(( a * b ))"
  array_index=$(( RANDOM % array_length ))
  ```

Control Flow and Conditionals
-----------------------------

* **Conditional statements**: Use `if` statements to execute code based on conditions.

  + Basic syntax: `if [[ CONDITION ]] then STATEMENTS fi`
  + Full syntax: `if [[ CONDITION ]] then STATEMENTS elif [[ CONDITION ]] then STATEMENTS else STATEMENTS fi`
  + Can use both `[[ ]]` and `(( ))` expressions for different types of conditions
  + **elif (else if)**: Optional, can be repeated multiple times to test additional conditions in sequence
  + **else**: Optional, executes when all previous conditions are false
  + Can mix double parentheses `(( ... ))` and double brackets `[[ ... ]]` in same conditional chain

  ```
  if (( NUMBER <= 15 ))
  then
      echo "B:$NUMBER"
  elif [[ $NUMBER -le 30 ]]
  then
      echo "I:$NUMBER"
  elif (( NUMBER < 46 ))
  then
      echo "N:$NUMBER"
  elif [[ $NUMBER -lt 61 ]]
  then
      echo "G:$NUMBER"
  else
      echo "O:$NUMBER"
  fi
  ```

Command Execution and Process Control
-------------------------------------

* **Command separation**: Use semicolon (`;`) to run multiple commands on a single line.

  + Commands execute sequentially from left to right
  + Each command's exit status can be checked individually

  ```
  [[ 4 -ge 5 ]]; echo $?
  ls -l; echo "Done"
  ```
* **Exit status**: Every command has an exit status that indicates success or failure.

  + Access exit status of the last command with `$?`
  + Exit status `0` means success (true/no errors)
  + Any non-zero exit status means failure (false/errors occurred)
  + Common error codes: `127` (command not found), `1` (general error)

  ```
  echo $?
  [[ 4 -le 5 ]]; echo $?
  ls; echo $?
  bad_command; echo $?
  ```
* **Subshells and command substitution**: Different uses of parentheses for execution contexts.

  + Single parentheses `( ... )` create a subshell
  + `$( ... )` performs command substitution
  + Subshells run in separate environments and don't affect parent shell variables

  ```
  ( cd /tmp; echo "Current dir: $(pwd)" )
  current_date=$(date)
  file_count=$(ls | wc -l)
  echo "Today is $current_date"
  echo "Found $file_count files"
  ```
* **Sleep command**: Pause script execution for a specified number of seconds.

  + Useful for creating delays in scripts
  + Can be used with decimal values for subsecond delays

  ```
  sleep 3
  sleep 0.5
  sleep 1
  ```

Loops
-----

* **While loops**: Execute code repeatedly while a condition is true.

  + Syntax: `while [[ CONDITION ]] do STATEMENTS done`

  ```
  I=5
  while [[ $I -ge 0 ]]
  do
      echo $I
      (( I-- ))
      sleep 1
  done
  ```
* **Until loops**: Execute code repeatedly until a condition becomes true.

  + Syntax: `until [[ CONDITION ]] do STATEMENTS done`

  ```
  until [[ $QUESTION =~ \?$ ]]
  do
      echo "Please enter a question ending with ?"
      read QUESTION
  done
  until [[ $QUESTION =~ \?$ ]]
  do
      GET_FORTUNE again
  done
  ```
* **For loops**: Iterate through arrays or lists using `for` loops with `do` and `done` to define the loop's logical block.

  ```
  for server in "${servers[@]}"
  do
      echo "Processing $server"
  done
  for (( i = 1; i <= 5; i++ ))
  do
      echo "Number: $i"
  done
  for (( i = 5; i >= 1; i-- ))
  do
      echo "Countdown: $i"
  done
  for i in {1..5}
  do
      echo "Count: $i"
  done
  ```

Arrays
------

* **Arrays**: Store multiple values in a single variable.

  + Create arrays with parentheses: `ARRAY=("value1" "value2" "value3")`
  + Access elements by index: `${ARRAY[0]}`, `${ARRAY[1]}`
  + Access all elements: `${ARRAY[@]}` or `${ARRAY[*]}`
  + Array indexing starts at 0

  ```
  RESPONSES=("Yes" "No" "Maybe" "Ask again later")

  echo ${RESPONSES[0]}     # Yes          
  echo ${RESPONSES[1]}     # No         
  echo ${RESPONSES[5]}     # Index 5 doesn't exist; empty string              
  echo ${RESPONSES[@]}     # Yes No Maybe Ask again later   
  echo ${RESPONSES[*]}     # Yes No Maybe Ask again later
  ```
* **Array inspection with declare**: Use `declare -p` to view array details.

  + Shows the array type with `-a` flag
  + Displays all array elements and their structure

  ```
  ARR=("a" "b" "c")
  declare -p ARR # ARR=([0]="a" [1]="b" [2]="c")
  ```
* **Array expansion**: Use `"${array_name[@]}"` syntax to expand an array into individual elements.

```
for server in "${servers[@]}"
```

Functions
---------

* **Functions**: Create reusable blocks of code.

  + Define with `FUNCTION_NAME() { STATEMENTS }`
  + Call by using the function name
  + Can accept arguments accessible as `$1`, `$2`, etc.

  ```
  GET_FORTUNE() {
      echo "Ask a question:"
      read QUESTION
  }
  GET_FORTUNE
  ```
* **Function arguments**: Functions can accept arguments just like scripts.

  + Arguments are passed when calling the function
  + Access arguments inside function using `$1`, `$2`, etc.
  + Use conditional logic to handle different arguments

  ```
  GET_FORTUNE() {
      if [[ ! $1 ]]
      then
          echo "Ask a yes or no question:"
      else
          echo "Try again. Make sure it ends with a question mark:"
      fi
      read QUESTION
  }
  GET_FORTUNE
  GET_FORTUNE again
  ```

Random Numbers and Mathematical Operations
------------------------------------------

* **Random numbers**: Generate random values using the `$RANDOM` variable.

  + `$RANDOM` generates numbers between 0 and 32767
  + Use modulo operator to limit range: `$RANDOM % 75`
  + Add 1 to avoid zero: `$(( RANDOM % 75 + 1 ))`
  + Must use `$(( ... ))` syntax for calculations with `$RANDOM`

  ```
  NUMBER=$(( RANDOM % 6 ))
  DICE=$(( RANDOM % 6 + 1 ))
  BINGO=$(( RANDOM % 75 + 1 ))
  echo $(( RANDOM % 10 ))
  ```
* **Random array access**: Use random numbers to access array elements randomly.

  + Generate random index within array bounds
  + Use random index to access array elements
  + Useful for random selections from predefined options

  ```
  RESPONSES=("Yes" "No" "Maybe" "Outlook good" "Don't count on it" "Ask again later")
  N=$(( RANDOM % 6 ))
  echo ${RESPONSES[$N]}
  ```
* **Modulo operator**: Use `%` to get the remainder of division operations.

  + Essential for limiting random number ranges
  + Works with `$RANDOM` to create bounded random values
  + `RANDOM % n` gives numbers from 0 to n-1

  ```
  echo $(( 15 % 4 ))
  echo $(( RANDOM % 100 ))
  echo $(( RANDOM % 10 + 1 ))
  ```

Environment and System Information
----------------------------------

* **Environment variables**: Predefined variables available in the shell environment.

  + `$RANDOM`: Generates random numbers between 0 and 32767
  + `$LANG`: System language setting
  + `$HOME`: User's home directory path
  + `$PATH`: Directories searched for executable commands
  + View all with `printenv` or `declare -p`

  ```
  echo $RANDOM
  echo $HOME
  echo $LANG
  printenv
  ```
* **Variable inspection**: Use `declare` to view and work with variables.

  + `declare -p`: Print all variables and their values
  + `declare -p VARIABLE`: Print specific variable details
  + Shows variable type (string, array, etc.) and attributes

  ```
  declare -p
  declare -p RANDOM
  declare -p MY_ARRAY
  ```
* **Command types**: Different categories of commands available in bash.

  + **Built-in commands**: Executed directly by the shell (e.g., `echo`, `read`, `if`)
  + **External commands**: Binary files in system directories (e.g., `ls`, `sleep`, `bash`)
  + **Shell keywords**: Language constructs (e.g., `then`, `do`, `done`)
  + Use `type <command>` to see what type a command is

  ```
  type echo
  type ls
  type if
  type ./script.sh
  ```

File Creation and Management
----------------------------

* **File creation**: Use `touch` to create new empty files.

  + Creates a new file if it doesn't exist
  + Updates the timestamp if the file already exists
  + Commonly used to create script files before editing

  ```
  touch script.sh
  touch bingo.sh
  touch filename.txt
  ```

Creating and Running Bash Scripts
---------------------------------

* **Script execution methods**: Multiple ways to run bash scripts:
  + **`sh scriptname.sh`**: Run with the sh shell interpreter.
  + **`bash scriptname.sh`**: Run with the bash shell interpreter.
  + **`./scriptname.sh`**: Execute directly (requires executable permissions).

```
sh questionnaire.sh
bash questionnaire.sh
./questionnaire.sh
```

File Permissions and Script Execution
-------------------------------------

* **Permission denied error**: When using `./scriptname.sh`, you may get "permission denied" if the file lacks executable permissions.
* **Checking permissions**: Use `ls -l` to view file permissions.

  ```
  ls -l questionnaire.sh
  ```
* **Permission format**: The output shows permissions as `-rw-r--r--` where:

  + First character (`-`): File type (- for regular file, d for directory)
  + Next 9 characters: Permissions for owner, group, and others
  + `r` = read, `w` = write, `x` = execute
* **Adding executable permissions**: Use `chmod +x` to give executable permissions to everyone.

  ```
  chmod +x questionnaire.sh
  ```
* **Script organization**: Best practices for structuring bash scripts.

  + Start with shebang (`#!/bin/bash`)
  + Add descriptive comments about script purpose
  + Define variables at the top
  + Group related functions together
  + Main script logic at the bottom

  ```
  #!/bin/bash
  NAME="value"
  ARRAY=("item1" "item2")
  my_function() {
      echo "Function code here"
  }
  my_function
  echo "Script complete"
  ```
* **Sequential script execution**: Create master scripts that run multiple programs in sequence.

  + Useful for automating workflows that involve multiple scripts
  + Each script runs to completion before the next one starts
  + Can combine different programs into a single execution flow
  + Arguments can be passed to individual scripts as needed
  + Can include different types of programs (interactive, automated, etc.)

  ```
  #!/bin/bash
  ./setup.sh
  ./interactive.sh
  ./processing.sh
  ./cleanup.sh
  ```

Database Normalization
----------------------

This is the process of organizing a relational database to reduce data redundancy and improve integrity.

Its benefits include:

* Minimizing duplicated data, which saves storage and reduces inconsistencies.
* Enforcing data integrity through the use of primary and foreign keys.
* Making databases easier to maintain and understand.

### Normal Forms

* **1NF (First Normal Form)**

  + Each cell contains a single (atomic) value.
  + Each record is unique (enforced by a primary key).
  + Order of rows/columns is irrelevant.
  + Example: Move multiple phone numbers from a `students` table into a separate `student_phones` table.
* **2NF (Second Normal Form)**

  + Meets 1NF requirements.
  + No **partial dependencies**: every non-key attribute must depend on the entire composite primary key.
  + Example: Split `orders` table into `order_header` and `order_items` to avoid attributes depending on only part of the key.
* **3NF (Third Normal Form)**

  + Meets 2NF requirements.
  + No **transitive dependencies**: non-key attributes cannot depend on other non-key attributes.
  + Example: Move `city_postal_code` to a `cities` table instead of storing it with every order.
* **BCNF (Boyce-Codd Normal Form)**

  + Meets 3NF requirements.
  + Every determinant (left-hand side of a functional dependency) must be a superkey.

**Tip**: Aim for 3NF in most designs for a good balance of integrity and performance.

Key SQL Concepts
----------------

* SQL is a Structured Query Language for communicating with relational databases.
* **Basic commands** → `SELECT`, `INSERT`, `UPDATE`, `DELETE`, `CREATE TABLE`, `ALTER TABLE`, etc.
* `Joins` → Combines data from multiple tables (`INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `FULL JOIN`).

Running SQL Commands in Bash
----------------------------

You can run SQL commands directly from the command line using the `psql` command-line client for PostgreSQL or similar tools for other databases.

For example, to run a SQL file in PostgreSQL:

```
psql -U username -d database_name -c "SELECT * FROM students;"
```

You can also execute MySQL commands directly:

```
mysql -u username -p database_name -e "SELECT * FROM students;"
```

### Run SQL from a File

```
# PostgreSQL
psql -U username -d database_name -f script.sql

# MySQL
mysql -u username -p database_name < script.sql
```

### Embed SQL in a Bash Script

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"

# Insert student data
psql -U "$DB_USER" -d "$DB_NAME" -c \
"INSERT INTO students (name, age, major) VALUES ('Alice', 20, 'CS');"
```

### Use of Variables in SQL

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"
STUDENT_NAME="Bob"
AGE=21

psql -U "$DB_USER" -d "$DB_NAME" -c \
"INSERT INTO students (name, age) VALUES ('$STUDENT_NAME', $AGE);"
```

**Tip**: Sanitize variables to avoid SQL injection.

Retrieving and Using SQL Query Results in Bash
----------------------------------------------

When you run SQL queries via `psql`, you can **capture** and **process** the returned values in your Bash scripts.

### Capturing a Single Value

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"

# Get total student count
STUDENT_COUNT=$(psql -U "$DB_USER" -d "$DB_NAME" -t -A -c \
"SELECT COUNT(*) FROM students;")

echo "Total students: $STUDENT_COUNT"
```

Output → 42

### Retrieving Multiple Columns

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"

# Get top 3 students' names and ages
RESULTS=$(psql -U "$DB_USER" -d "$DB_NAME" -t -A -F"," -c \
"SELECT name, age FROM students LIMIT 3;")

echo "Top 3 students:"
echo "$RESULTS"
```

Output

```
Alice,20
Bob,21
Charlie,22
```

### Looping Through Query Results

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"

# Get student names and majors
psql -U "$DB_USER" -d "$DB_NAME" -t -A -F"," -c \
"SELECT name, major FROM students;" | while IFS="," read -r name major
do
    echo "Student: $name | Major: $major"
done
```

Shape of Output

```
Student: Alice | Major: CS
Student: Bob   | Major: Math
Student: Carol | Major: Physics
```

SQL Injection
-------------

It is a web security vulnerability where attackers insert malicious SQL code into input fields to manipulate the database.

This can lead to risky actions like:

* Bypassing authentication.
* Stealing sensitive data.
* Modifying or deleting records.

An example of an SQL injection attack:

```
SELECT * FROM users WHERE username = ' " " OR "1"="1" -- ' AND password = 'anything';
```

This query would return all users because the condition `OR "1"="1"` is always true, allowing attackers to bypass login checks.

### Preventing SQL Injection

1. **Use Prepared Statements**: These separate SQL code from data, preventing injection. Here's an example (Node.js with pg):

   ```
   client.query('SELECT * FROM users WHERE username = $1 AND password = $2', [username, password]);
   ```
2. **Input Validation**: Sanitize and validate all user inputs to ensure they conform to expected formats.
3. **Least Privilege**: Use database accounts with the minimum permissions necessary for the application.

**Note**: Never grant admin rights to application accounts.

N+1 Problem
-----------

The N+1 problem occurs when an application makes one query to retrieve a list of items (N) and then makes an additional query for each item to retrieve related data, resulting in N+1 queries.

**Why It's Bad**

* Each query adds network and processing overhead.
* Multiple small queries are slower than one optimized query.

### Example of N+1 Pattern

```
-- 1: Get list of orders
SELECT * FROM orders LIMIT 50;

-- N: For each order, get customer
SELECT * FROM customers WHERE customer_id = ...;
```

**Solution**: Use `JOINs` or other set-based operations.

```
SELECT 
  orders.order_id,
  orders.product,
  orders.quantity,
  customers.customer_id,
  customers.name,
  customers.email,
  customers.address
FROM orders
JOIN customers 
  ON orders.customer_id = customers.customer_id
WHERE orders.order_id IN (SELECT order_id FROM orders LIMIT 50);
```

Always look for opportunities to combine related data into a single query.

Introduction to Version Control
-------------------------------

* **Definition**: A version control system allows you to track and manage changes in your project. Examples of version control systems used in software are Git, SVN, or Mercurial.

Cloud-Based Version Control Providers
-------------------------------------

* **List of Cloud-Based Version Control Providers**: GitHub and GitLab are popular examples of cloud-based version control providers that allow software teams to collaborate and manage repositories.

Installing and Setting up Git
-----------------------------

* **Installing Git**: To check if Git is already installed on your machine you can run the following command in the terminal:

```
git --version
```

If you see a version number, that means Git is installed. If not, then you will need to install it.

For Linux systems, Git often comes preinstalled with most distros. If you do not have Git pre-installed, you should be able to install it with your package manager commands such as `sudo apt-get install git` or `sudo pacman -S git`.

For Mac users, you can install Git via Homebrew with `brew install git`, or you can download the executable installer from Git's website.

For Windows, you can download the executable installer from Git's website. Or, if you have set up Chocolatey, you can run `choco install git.install` in PowerShell. Note that on Windows, you may also want to download Git Bash so you have a Unix-like shell environment available.

To make sure the installation worked, run the `git --version` command again in the terminal.

* **Git Configurations**: `git config` is used to set configuration variables that are responsible for how Git operates on your machine. To view your current setting variables and where they are stored on your system, you can run the following command:

```
git config --list --show-origin
```

Right now you should be seeing only system-level configuration settings if you just installed Git for the first time.

To set your user name, you can run the following command:

```
git config --global user.name "Jane Doe"
```

The `--global` flag is used here to set the user name for all projects on your system that use Git. If you need to override the user name for a particular project, then you can run the command in that particular project directory without the `--global` flag.

To set the user email address, you can run the following command:

```
git config --global user.email janedoe@example.com
```

Another configuration you can set is the preferred editor you want Git to use. Here is an example of how to set your preferred editor to Emacs:

```
git config --global core.editor emacs
```

If you choose not to set a preferred editor, then Git will default to your system's default editor.

Open vs. Closed Source Software
-------------------------------

* **Definition**: "Open-source" means people can see the code you publish, propose changes, report issues, and even run a modified version. "Closed-source" means the only people who can see and interact with the project are the people you explicitly authorize.

GitHub
------

* **Definition**: GitHub is a cloud-based solution that offers storage of version-controlled projects in something called "repositories", and enables collaboration features to use with those projects.
* **GitHub CLI**: This tool is used to do GitHub-specific tasks without leaving the command line. If you do not have it installed, you can get instructions to do so from GitHub's documentation - but you should have it available in your system's package manager.
* **GitHub Pages**: GitHub Pages is an option for deploying static sites, or applications that do not require a back-end server to handle logic. That is, applications that run entirely client-side, or in the user's browser, can be fully deployed on this platform.
* **GitHub Actions**: GitHub Actions is a feature that lets you automate workflows directly in your GitHub repository including building, testing, and deploying your code.

Common Git Commands
-------------------

* **`git init`**: This will initialize an empty Git repository so Git can begin tracking changes for this project. When you initialize an empty Git repository to a project, a new `.git` hidden directory will be added. This `.git` directory contains important information for Git to manage your project.
* **`git status`**: This command is used to show the current state of your working directory - you will be using this command a lot in your workflow.
* **`git add`**: This command is used to stage your changes. Anything in the staging area will be added for the next commit. If you want to stage all unstaged changes, then you can use `git add .` The period (`.`) is an alias for the current directory you are in.
* **`git commit`**: This command is used to commit your changes. A commit is a snapshot of your project state at that given time. If you run `git commit`, it will open up your preferred editor you set in the Git configuration. Once the editor is open, you can provide a detailed message of your changes. You can also choose to provide a shorter message by using the `git commit -m` command like this:

```
git commit -m "short message goes here"
```

* **`git log`**: This will list all prior commits with helpful information like the author, date of commit, commit message and commit hash. The commit hash is a long string which serves as a unique identifier for a commit.
* **`git remote add`**: This command is used to setup the remote connection to your remote repo.
* **`git push`**: This command is used to push up your changes to a remote repository.
* **`git pull`**: This command is used to pull down the latest changes from your remote repository into your local repository.
* **`git clone`**: This command will clone a repository. This means you will have a copy of the repository. This copy includes the repository history, all files/folders and commits on your local device.
* **`git remote -v`**: This command will show the list of remote repositories associated with your local Git repository.
* **`git branch`**: This command will list all of your local branches.
* **`git fetch upstream`**: This command tells Git to go get the latest changes that are on your upstream remote (which is the original repo).
* **`git merge upstream/main`**: This command tells Git to merge the latest changes from the `main` branch in the upstream remote into your current branch.
* **`git reset`**: This command allows you to reset the current state of a branch. Passing the `--hard` flag tells Git to force the local files to match the branch state. This ensures that you have a clean slate to work from.
* **`git rebase`**: A rebase in Git is a way to move or combine a sequence of commits from one branch onto another.

Working with Branches
---------------------

* **Definition**: A branch in Git is a separate workspace where you can make changes. The `main` branch will often represent the primary or production branch in a real world application. Developer teams will create multiple branches for new features and bug fixes and then merge those changes back into the `main` branch.
* **Creating a New Branch**: To create a new branch you can run the following command:

```
git branch feature
```

To checkout that branch, you can run the following command:

```
git checkout feature
```

Most developers will use the shorthand command for creating and checking out a branch which is the following:

```
git checkout -b new-branch-name
```

A newer and alternative command would be the `git switch` command. Here is an example for creating and switching to a new branch:

```
git switch -c new-branch-name
```

* **Branching Strategies**: Your `main` branch is your default branch and usually is pretty stable. So it is best to branch off from there to create new branches for items like bug fixes, new features, or other miscellaneous work.
* **Merge Conflicts**: This happens when Git tries to automatically merge changes from different branches but can't decide which changes to keep. This usually happens when there are conflicting changes for the same portion of the file.

Five States for a Git Tracked File
----------------------------------

* **"Untracked"**: This means that the file is new to the repository, and Git has not "seen" it before.
* **"Modified"**: This file existed in the previous commit, and has changes that have not been committed.
* **"Ignored"**: You likely won't see ignored files in Git, but your IDE might have an indicator for them. Ignored files are excluded from Git operations, typically because they are included in the `.gitignore` file.
* **"Deleted"**: A deleted file is the opposite of an untracked file - it's a file that previously existed, and has been removed.
* **"Renamed"**: A renamed file is a file where the contents are unchanged, but the name or location of the file was modified. In some cases, a file can be considered renamed even if it has a small amount of changes.

`.gitignore` Files
------------------

* **Definition**: The `.gitignore` file is a special type of file related to Git operations. The name suggests that this file is used to tell Git to ignore things, and that's the common use case. But what it actually does is it tells Git to stop tracking a file.

Working with Repositories
-------------------------

* **Definition**: A repository is like a container for a project - if you are working on an app, you would keep the files for that app together in a repository. Repositories can be local on your computer, or remote on a service like GitHub.
* **Public vs. Private Repositories**: A public repository can be viewed and downloaded by anyone. A private repository can only be accessed by you, and anyone you grant explicit access to.
* **Creating Repositories on GitHub**: To create a new repository on GitHub, you can click on the `"New Repository"` button and walk through the GitHub UI of setting up a new repository.
* **Pushing Local Repositories to GitHub**: If you have a local project on your computer, you can push up that repository to GitHub. Here is a step-by-step overview of the process:

1. Initialize an empty git repository in the project directory (`git init`).
2. Make changes to your project.
3. Run the `git status` command to see all changes made that are being tracked by git.
4. Stage your changes (`git add`).
5. Commit your changes (`git commit`).
6. Setup the remote connection (`git remote add`).
7. Push your changes to GitHub (`git push`).

Pull Requests
-------------

* **Pull Requests**: A pull request is a request to pull changes in from your branch into the target branch. Pull requests are the flow you use when you want to contribute code changes to a project. This approach allows the maintainers of the project to review your changes. They can leave comments, ask questions, and suggest tweaks. Then once the review process is complete, it can be approved and merged into the main branch.

Contributing to Other Repositories
----------------------------------

* **Process**: There are thousands of projects that you can contribute to. Here is the basic process on how to contribute to another repository:

1. Read the contributing documentation
2. Find an available issue to work on
3. Fork the repository
4. Clone your forked copy of the repository
5. Create a new branch
6. Make the changes according to the issue
7. Create a PR (Pull Request)
8. Wait for a review for that PR

Working with SSH and GPG Keys
-----------------------------

* **GPG Keys**: GPG, or Gnu Privacy Guard, keys are typically used to sign files or commits. Someone can then use your public GPG key to verify that the file signature is from your key and that the contents of the file have not been modified or tampered with.

To generate a GPG key, you'll need to run:

```
gpg --full-generate-key
```

* **SSH Keys**: SSH, or Secure SHell, keys are typically used to authenticate a remote connection to a server - via the `ssh` utility. You can also use an SSH key to sign commits.

For an SSH key, you'll run:

```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

`ed25519` is a modern public-key signature algorithm.

* **Signing Commits with GPG Keys**: In order to sign your commits with your GPG key, you'll need to upload your public key, not the private key, to your GitHub account. To list your public keys, you will need to run the following:

```
gpg --list-secret-keys --keyid-format=long
```

Then, to get the public key, use:

```
gpg --armor --export "<key id>"
```

Then, take the short ID you got from listing the keys and run this command to set it as your git signing key:

```
git config --global user.signingkey <your_gpg_key_id>
```

Then, you can pass the `-S` flag to your `git commit` command to sign a specific commit - you'll need to provide your passphrase. Alternatively, if you want to sign every commit automatically, you can set the autosign config to `true`:

```
git config --global commit.gpgsign true
```

* **Signing Commits with SSH Keys**: To sign with an SSH key, which is a relatively new feature on GitHub, you'll need to start by uploading the key to your GitHub account. Then you'll need to set the signing mode for git to use SSH:

```
git config --global gpg.format ssh
```

Then, to set the signing key, you'll pass the file path instead of an ID:

```
git config --global user.signingkey <path_to_your_ssh_keys>
```

---

### Section Summary: Sql And Postgresql

# SQL and PostgreSQL Review

Introduction to Relational Databases
------------------------------------

* **Relational Databases**: Organize data into related tables made of rows and columns. Each row represents a record, and each column represents an attribute of the data.
* **Advantages of Relational Databases**: Scalable, widely applicable across domains (e.g., healthcare, business, gaming), and structured to maintain reliable data.
* **Common Use Cases**: Web development, inventory systems, e-commerce, healthcare, and enterprise applications.

Key Concepts
------------

* **Schema**: A relational database requires a schema that defines its structure—tables, columns, data types, constraints, and relationships.
* **Primary Keys**: Unique identifiers for each row in a table. They are essential for data integrity and are used to relate records between tables via foreign keys.
* **Foreign Keys**: References to primary keys in another table, used to link related data across tables.
* **Relationships**: By connecting tables through primary and foreign keys, you can structure normalized data and perform meaningful queries.
* **Entity Relationship Diagrams (ERDs)**: Visualize how entities (tables) relate to each other in a database schema.
* **Data Integrity**: Enforced using keys and data types. Ensures consistency and accuracy of stored data.

SQL Basics
----------

* **Queries**: Requests to retrieve specific data from the database.

```
SELECT * FROM dogs WHERE age < 3;
```

* **WHERE clause**: Filter results based on conditions. Use comparison operators like `<`, `=`, `>`, etc.
* **Select with ORDER BY**: Retrieve and sort results based on a column.

```
SELECT columns FROM table_name ORDER BY column_name;
```

Table Operations
----------------

* **`CREATE TABLE` Statement**: This statement is used to create a new table in a database.

```
CREATE TABLE first_table();
```

* **`ALTER TABLE ADD COLUMN` Statement**: This statement is used to add a column to an existing table.

```
ALTER TABLE table_name ADD COLUMN column_name DATATYPE;
```

* **`ALTER TABLE DROP COLUMN` Statement**: This statement is used to drop a column from an existing table.

```
ALTER TABLE table_name DROP COLUMN column_name;
```

* **`ALTER TABLE RENAME COLUMN` Statement**: This statement is used to rename a column in a table.

```
ALTER TABLE table_name RENAME COLUMN column_name TO new_name;
```

* **`DROP TABLE` Statement**: This statement is used to drop an entire table from the database.

```
DROP TABLE table_name;
```

* **`ALTER DATABASE RENAME` Statement**: This statement is used to rename a database.

```
ALTER DATABASE database_name RENAME TO new_database_name;
```

* **`DROP DATABASE` Statement**: This statement is used to drop an entire database.

```
DROP DATABASE database_name;
```

Constraints & Data Integrity
----------------------------

* **`ALTER TABLE ADD COLUMN` with Constraint**: This statement is used to add a column with a constraint to an existing table.

```
ALTER TABLE table_name ADD COLUMN column_name DATATYPE CONSTRAINT;
```

* **`NOT NULL` Constraint**: This constraint ensures that a column cannot have NULL values.

```
column_name VARCHAR(50) NOT NULL
```

* **`ALTER TABLE ADD PRIMARY KEY` Statement**: This statement is used to add a primary key constraint to a table.

```
ALTER TABLE table_name ADD PRIMARY KEY(column_name);
```

* **`ALTER TABLE DROP CONSTRAINT` Statement**: This statement is used to drop a constraint from a table.

```
ALTER TABLE table_name DROP CONSTRAINT constraint_name;
```

* **`ALTER TABLE ADD COLUMN` with Foreign Key**: This statement is used to add a foreign key column that references another table.

```
ALTER TABLE table_name ADD COLUMN column_name DATATYPE REFERENCES referenced_table_name(referenced_column_name);
```

* **`ALTER TABLE ADD UNIQUE` Statement**: This statement is used to add a UNIQUE constraint to a column.

```
ALTER TABLE table_name ADD UNIQUE(column_name);
```

* **`ALTER TABLE ALTER COLUMN SET NOT NULL` Statement**: This statement is used to set a NOT NULL constraint on an existing column.

```
ALTER TABLE table_name ALTER COLUMN column_name SET NOT NULL;
```

* **`INSERT` Statement with NULL Values**: This statement demonstrates how to insert NULL values into a table.

```
INSERT INTO table_name(column_a) VALUES(NULL);
-- or
INSERT INTO table_name(column_b) VALUES('value'); -- if column_a allows nulls
```

* **Composite Primary Key**: This constraint defines a primary key that consists of multiple columns.

```
CREATE TABLE course_enrollments (
    student_id INT,
    course_id INT,
    PRIMARY KEY (student_id, course_id)
);
```

Data Manipulation (CRUD)
------------------------

* **`INSERT` Statement**: This statement is used to insert a single row into a table.

```
INSERT INTO table_name(column_1, column_2) VALUES(value1, value2);
```

* **`INSERT` Statement with Omitted Columns**: This statement shows how to insert values without explicitly listing the column names, relying on the default column order in the table.

```
INSERT INTO dogs VALUES ('Gino', 3);
```

* **`INSERT` Statement with Multiple Rows**: This statement is used to insert multiple rows into a table in a single operation.

```
INSERT INTO dogs (name, age) VALUES 
('Gino', 3),
('Nora', 2);
```

* **`UPDATE` Statement**: This statement is used to update existing data in a table based on a condition.

```
UPDATE table_name SET column_name=new_value WHERE condition;
```

* **`DELETE` Statement**: This statement is used to delete rows from a table based on a condition.

```
DELETE FROM table_name WHERE condition;
```

Data Types
----------

* **`NUMERIC` Data Type**: This data type is used to store precise decimal numbers with a specified precision and scale.

```
price NUMERIC(10, 2)
```

* **`TEXT` Data Type**: This data type is used to store variable-length character strings with no specific length limit.

```
column_name TEXT
```

* **`INTEGER` Data Type**: This data type is used to store whole numbers without decimal places.

```
units_sold INTEGER
```

* **`SMALLINT` and `BIGINT` Data Types**: These are variants of INTEGER with smaller and larger ranges respectively.
* **`SERIAL` Data Type**: This data type is used to create auto-incrementing integer columns in PostgreSQL.

```
id SERIAL
```

* **`AUTO_INCREMENT` Attribute**: This attribute is used in MySQL to create auto-incrementing integer columns.

```
id INT AUTO_INCREMENT
```

* **`VARCHAR` Data Type**: This data type is used to store variable-length character strings with a specified maximum length.

```
name VARCHAR(50)
```

* **`DATE` Data Type**: This data type is used to store date values (year, month, day).

```
event_date DATE
```

* **`TIME` Data Type**: This data type is used to store time values (hour, minute, second).

```
start_time TIME
```

* **`TIMESTAMP` Data Type**: This data type is used to store date and time values, optionally with time zone information.

```
event_timestamp TIMESTAMP
event_timestamp TIMESTAMP WITH TIME ZONE
```

* **`BOOLEAN` Data Type**: This data type is used to store true/false values.

```
is_active BOOLEAN
```

Database Relationships
----------------------

* **Types of Relationships**: These are the different ways tables can be related to each other in a relational database.

  + One-to-one
  + One-to-many
  + Many-to-one
  + Many-to-many
  + Self-referencing (recursive)
* **One-to-One Relationship**: This relationship type means that each record in one table corresponds to exactly one record in another table.

```
One employee is assigned exactly one vehicle.
Tables: employees, vehicles
```

* **One-to-Many Relationship**: This relationship type means that one record in a table can be associated with multiple records in another table.

```
One customer can have many orders.
Tables: customers → orders
```

* **Many-to-Many Relationship via Junction Table**: This relationship type is implemented using a junction table that contains foreign keys from both related tables.

```
CREATE TABLE books_authors (
    author_id INT REFERENCES authors(id),
    book_id INT REFERENCES books(id)
);
```

* **Self-Referencing Relationships**: This relationship type occurs when a table references itself, creating a hierarchical structure.

```
An employee table where each employee may report to another employee.
```

Advanced SQL (Joins)
--------------------

* **`INNER JOIN` Statement**: This join returns only the rows that have matching values in both tables.

```
SELECT *
FROM products
INNER JOIN sales ON products.product_id = sales.product_id;
```

* **`FULL OUTER JOIN` Statement**: This join returns all rows from both tables, including unmatched rows from either table.

```
SELECT *
FROM products
FULL OUTER JOIN sales ON products.product_id = sales.product_id;
```

* **`LEFT OUTER JOIN` Statement**: This join returns all rows from the left table and matching rows from the right table.

```
SELECT *
FROM products
LEFT JOIN sales ON products.product_id = sales.product_id;
```

* **`RIGHT OUTER JOIN` Statement**: This join returns all rows from the right table and matching rows from the left table.

```
SELECT *
FROM products
RIGHT JOIN sales ON products.product_id = sales.product_id;
```

* **`SELF JOIN` Statement**: This join is used to join a table with itself to compare rows within the same table.

```
SELECT A.column_name, B.column_name
FROM table_name A
JOIN table_name B ON A.related_column = B.related_column;
```

* **`CROSS JOIN` Statement**: This join returns the Cartesian product of two tables, combining every row from the first table with every row from the second table.

```
SELECT *
FROM table1
CROSS JOIN table2;
```

PostgreSQL Specific Commands
----------------------------

* **`psql` Login Command**: This command is used to log in to PostgreSQL with specific username and database.

```
psql --username=freecodecamp --dbname=postgres
```

* **`\l` Command**: This command lists all databases in the PostgreSQL instance.

```
\l
```

* **`CREATE DATABASE` and `\c` Commands**: These commands are used to create a new database and connect to it.

```
CREATE DATABASE database_name;
\c database_name
```

* **`\d` Command**: This command lists all tables in the current database.

```
\d
```

* **`\d table_name` Command**: This command displays the schema/structure of a specific table.

```
\d table_name
```

* **`\q` Command**: This command exits the PostgreSQL client.

```
\q
```

Relational vs Non-Relational
----------------------------

* **Non-Relational (NoSQL) Databases**: Store unstructured or semi-structured data. Do not require a rigid schema and are more flexible for evolving data models.
* **Choosing Between Relational and Non-Relational**: Depends on the nature of your data and application requirements.
* **Relational vs Non-Relational**: Choose relational for structured data and consistency; NoSQL for flexibility and fast-changing data.

Popular RDBMS Systems
---------------------

* **MySQL**: Open-source, reliable, widely used in web development, supported by a large community.
* **PostgreSQL**: Open-source, advanced, extensible. Supports custom data types and server-side programming.
* **SQLite**: Lightweight, file-based, serverless. Ideal for small applications.
* **Microsoft SQL Server**: Proprietary, enterprise-grade database.
* **Oracle Database**: Commercial RDBMS known for large-scale performance and scalability.

Best Practices
--------------

* **Naming Convention**: Use `snake_case` (e.g., `delivery_orders`) for table and column names.

---

## Module 6: Advanced SQL Concepts, Optimization, & Security

### Lecture 6.1: What Is Normalization In Sql

# What Is Normalization in SQL?

Normalization is the process of organizing a relational database using established normal forms to reduce data redundancy and improve data integrity.

To normalize a database, you analyze the attributes and relationships in your table structures to identify opportunities for simplification based on normalization rules. Then, you divide the data into smaller, more focused tables and establish relationships between them using primary and foreign keys. These smaller tables will store all the data that you originally had, but they will be easier to manage, organize, and work with, compared to larger tables.

By minimizing data redundancy, normalization reduces storage space and prevents inconsistencies. For example, if a customer's address changes, you only need to update it in one customer table rather than in every order record.

It also helps preserve data integrity by making sure that dependencies are enforced by primary and foreign key constraints. This reduces the likelihood of insertion, update, and deletion anomalies.

A normalized database is easier to understand and maintain, which contributes to a well-designed database system.

The set of rules that you should follow to organize your tables are called normal forms. Each normal form builds on the previous ones, with rules becoming stricter as you move to higher normal forms. The First Normal Form (1NF) is the foundational form, with the most basic rules.

A table is in First Normal Form (1NF) if:

* Each cell should contain only one value. For example, if you have a `students` table, you may have a student with multiple phone numbers. Instead of storing them as a comma-separated list in one cell, you should create a separate `phone_numbers` table with a foreign key pointing to the `students` table and only store one value in each cell. This keeps each value atomic and the design normalized.
* Every record (row) must be unique. While primary keys enforce this requirement, 1NF explicitly mandates that no duplicate rows exist in the table.
* The order of the rows and columns should not be relevant. Data should not depend on its physical location.

Essentially, the First Normal Form (1NF) focuses on making values simple and atomic.

The Second Normal Form (2NF) builds on 1NF, requiring that all 1NF requirements are met plus additional constraints.

Understanding 2NF requires familiarity with two key concepts: superkeys and candidate keys. A superkey is any set of attributes that uniquely identifies each row in a table, meaning no two rows can have identical values across all columns in the superkey.

For example, if we have a `customers` table with three columns:

```
customer_id | name | email
```

Let's say that `customer_id` and `email` must be unique for each record. Some examples of superkeys for this table would be:

* `customer_id`
* `{ customer_id, name }`, this combination uniquely identifies rows because `customer_id` alone is unique, regardless of `name`'s uniqueness.
* `{ customer_id, name, email }`
* `email`, since we are adding the unique constraint to this column too, each record can be uniquely identified by the email.

Any set of attributes that, together, identify each row can be a superkey.

A candidate key is similar and yet, a bit different. It's a set of one or more columns on the table that can uniquely identify each record. A table can have multiple candidate keys but you'll need to choose one to act as the primary key.

They sound quite similar, right? Their difference is that the superkey can also contain additional attributes that are not necessary to identify each row uniquely, while the candidate key only contains attributes that do identify the row uniquely.

In our `customers` example, we mentioned that `customer_id`, `{ customer_id, name }`, `{ customer_id, name, email }`, and `email` can be superkeys. In this case, only `customer_id` and `email` can be candidate keys because candidate keys can't include attributes that don't identify the row uniquely, like `name`. This illustrates the minimality principle that distinguishes candidate keys from superkeys.

Now that you're familiar with these concepts, let's go back to the Second Normal Form (2NF).

The Second Normal Form (2NF) is based on addressing partial dependencies. A partial dependency occurs in a table when an attribute that is not part of the primary key only depends on part of a composite primary key (a composite key is a primary key made of multiple columns). This can lead to data redundancy and update anomalies.

For example, let's say we have an `orders` table with these columns:

```
order_id | item_id | order_date | quantity | order_shipping_city
```

In this table, the primary key is the combination of `order_id` and `item_id` because the same item ID can be in different orders, but their combination will be unique. You can see that there is a partial dependency between `order_id` and `order_shipping_city`. `order_id` is part of the primary key. `order_shipping_city` depends on `order_id` because every order with the same ID will have the same shipping city. However, the shipping city does not depend on the `item_id`, but this is also part of the primary key. Therefore, `order_shipping_city` does not depend on the entire primary key.

To fix this, you can split the table into two smaller tables, like `order_header` and `order_items`. In the `order_header` table, you could store the top-level information about the orders:

```
order_id | order_date | order_shipping_city
```

In the `order_items` table, you could store information about the items in the different orders that were submitted:

```
order_id | item_id | quantity
```

With these changes, both tables will be in Second Normal Form (2NF).

And that leads us to the Third Normal Form (3NF). This normal form builds on the second normal form.

For a table to be in Third Normal Form, it must:

* Be in Second Normal Form.
* Have all non-key attributes depend directly on the primary key, meaning no non-key attribute should depend on another non-key attribute.

To understand the Third Normal Form (3NF), you need to understand transitive dependencies. A transitive dependency occurs when an attribute that is not part of the primary key depends on another attribute that is not part of the primary key, which in turn depends on the primary key.

For example, let's modify our `orders` table to have these columns:

```
order_id | customer_id | customer_city | city_postal_code | order_date | quantity
```

The primary key in this new table is `order_id` because it uniquely identifies each row.

There is a transitive dependency in this table:

```
order_id > customer_id > customer_city > city_postal_code
```

The city's postal code is determined by the customer's city, which is determined by the customer's ID, which is determined by the order's ID. `city_postal_code`, an attribute that is not part of the primary key, is determined by `customer_city`, which is also not part of the primary key, but `customer_city` is determined by `order_id` through `customer_id`. This means that the city's postal code will be repeated for every order placed by customers who live in the same city. This will lead to data redundancy. Additionally, any change to a city's postal code would require updates across multiple records.

To solve the transitive dependency, you would need to split the table into multiple tables. First, an `orders` table:

```
order_id | customer_id | order_date | quantity
```

Then, a `customers` table:

```
customer_id | city_name
```

And a `cities` table:

```
city_name | city_postal_code
```

This removes the transitive dependency from the table.

And finally, we have the Boyce-Codd Normal Form (BCNF). This is also known as Normal Form 3.5 because it addresses some anomalies that the Third Normal Form may not address. For a table to be in the Boyce-Codd Normal Form (BCNF), it has to:

* Be in Third Normal Form.
* Have every left-hand side of a functional dependency be a superkey.

The goal of this normal form is to ensure that every attribute or set of attributes that determines another attribute is a superkey, which is a candidate key or a superset of them.

Understanding and applying the normal forms is essential for designing robust and efficient relational databases. By eliminating data redundancy and ensuring logical data dependencies, normalization leads to improved data integrity, reduced storage requirements, and simplified database maintenance. You should usually aim to reach the Third Normal Form (3NF).

---

### Lecture 6.2: What Is The N Plus 1 Problem

# What Is the N+1 Problem?

The N+1 problem is a common performance bottleneck in database-driven applications. If you've ever experienced a really long load time while using an application, it's very likely related to the N+1 problem. This problem occurs when many small queries are being performed in a sequence to get the data you requested.

But why would you perform many queries in a sequence? You might do this to query a list of records and additional information about those records. You would perform an initial query to get the list of records and then perform an additional query for each one of those records, to get additional information about them.

Even if you intuitively think that performing many small and simple queries will be more efficient than performing just one large and complex query, this is usually not the case. The more queries you perform, the longer the entire process will take because you need to send each query to the server, find the data on the database, and then receive the data sent by the server for that query. This can have a very significant performance impact on your application.

To show you a practical example, let's say you're developing an application for a food delivery service and you run a query to get the first 50 orders in the database. First, you will get a list with these orders from an `orders` table, like this one:

```
order_id | product   | quantity | customer_id
1        | pizza     | 2        | 3422
2        | salad     | 1        | 1255
3        | ice cream | 4        | 2344
4        | donuts    | 10       | 3455
.        | .         | .        | .
.        | .         | .        | .
.        | .         | .        | .
```

But what if you also need to get the data of the customers who submitted these orders? This information would be stored in a different `customers` table.

One way to approach this would be to get the list of orders first and then run one query per order to get the customers' information. To get the list of orders, you could run a query like this one, to get the first 50 records from the `orders` table:

```
SELECT * FROM orders LIMIT 50;
```

This is where the 1 in N+1 comes from. It's the initial query that gives you the list of records. Then, you will need to perform another query for each one of these records to get the information of the customer who submitted the order. For this, you might write a loop in an asynchronous function to process both orders and customers. The `getCustomerData()` function will perform a SQL query to get the data of the customer who placed a specific order. It will do this in a sequence for each order that was placed:

```
for (const order of orders) {
  const customerId = order.customer_id;
  const customerData = await getCustomerData(customerId);
  // Process the customer's data.
}
```

That's where the N in N+1 comes from. N represents the number of queries that will be performed to get additional data for each one of the records.

This approach might seem simple and intuitive, but you might be surprised to know that this is exactly what you shouldn't do. You should avoid making queries in a loop because making multiple small queries will take much longer than performing a single, larger query to get all the data.

You should try to use the tools that SQL gives you to reduce the number of queries as much as possible. In this case, we could use a `JOIN` operation to join the `orders` and `customers` table.

```
SELECT 
  orders.order_id,
  orders.product,
  orders.quantity,
  customers.customer_id,
  customers.name AS customer_name,
  customers.email AS customer_email,
  customers.address AS customer_address
FROM orders
JOIN customers ON orders.customer_id = customers.customer_id
WHERE orders.order_id IN (SELECT order_id FROM orders LIMIT 50)
```

With the `JOIN` operation, we can retrieve the data of the first 50 orders in the database, including the data of the customers, their names, email, and addresses, with only one query. It might look more complex, but it's actually more efficient this way.

Now you know what the N+1 problem involves, so you can identify it and prevent it, to interact with your database in an efficient way.

---

### Lecture 6.3: What Is Sql Injection And What Are Some Ways To Prevent It

# What Is SQL Injection, and What Are Some Ways to Prevent It?

SQL injection is a web security vulnerability in which attackers change or take advantage of the queries that the web application makes to the database. For example, attackers can insert malicious SQL code into the query to run the malicious code on the back-end.

This can happen when you give users the option to enter data through login forms, search bars, or URL parameters and then use that user input in string interpolation or concatenation to generate the final SQL command.

Depending on the attacker's goal, the malicious SQL code can cause significant disruptions on your database and web application, like bypassing authentication, stealing data from the database, or modifying or removing database records. Therefore, you should take this threat very seriously.

For example, let's say your web application uses an SQL query like this one to authenticate users, directly embedding the username and password entered by the user:

```
'SELECT * FROM users WHERE username = ' + username_input + ' AND password = ' + password_input + ';'
```

If an attacker enters something like this to the `username` field:

```
'" " OR "1"="1" --'
```

And anything else in the `password` field, since `"1"="1"` is always `true` and `--` comments out the rest of the query, the `WHERE` clause becomes:

```
WHERE username = " " OR TRUE
```

Which is always `true`.

Depending on the database implementation, this may return the data of the first user or any user in the database and allow the attacker to log in without valid credentials.

So how can you prevent this? There are two main ways to prevent SQL injection:

* Don't write dynamic queries with string concatenation.
* And prevent malicious SQL input from being included in queries that will be executed in the back-end.

In practice, you can use parameterized statements, also known as parameterized queries. They separate the SQL structure from the data entered by the user, which prevents the database from interpreting the input data as executable code.

Another important technique is input validation. This is recommended as a secondary security measure in all cases, but it's specially important for parts of SQL queries related to table names, column names, and sorting order. If possible, it's recommended to assign table names and column names directly within your code, not from user input.

If, despite all the preventive measures, you do get an SQL injection attack, you can minimize its impact on the database by limiting the permissions of each database account. Grant each database user only the permissions needed for their tasks, but nothing more. If an account only needs to read data from the database, grant it read access only. And as a preventive measure, never assign admin permissions to your application accounts. It is very dangerous to do so because an attacker could get complete access and full control over the database.

SQL injection is a very common attack that you, as a developer, should be aware of and prevent in the implementation of your web application. With these techniques, you can protect your database and keep your user's data safe.

---

### Section Summary: Bash And Sql

# Bash and SQL Review

Database Normalization
----------------------

This is the process of organizing a relational database to reduce data redundancy and improve integrity.

Its benefits include:

* Minimizing duplicated data, which saves storage and reduces inconsistencies.
* Enforcing data integrity through the use of primary and foreign keys.
* Making databases easier to maintain and understand.

### Normal Forms

* **1NF (First Normal Form)**

  + Each cell contains a single (atomic) value.
  + Each record is unique (enforced by a primary key).
  + Order of rows/columns is irrelevant.
  + Example: Move multiple phone numbers from a `students` table into a separate `student_phones` table.
* **2NF (Second Normal Form)**

  + Meets 1NF requirements.
  + No **partial dependencies**: every non-key attribute must depend on the entire composite primary key.
  + Example: Split `orders` table into `order_header` and `order_items` to avoid attributes depending on only part of the key.
* **3NF (Third Normal Form)**

  + Meets 2NF requirements.
  + No **transitive dependencies**: non-key attributes cannot depend on other non-key attributes.
  + Example: Move `city_postal_code` to a `cities` table instead of storing it with every order.
* **BCNF (Boyce-Codd Normal Form)**

  + Meets 3NF requirements.
  + Every determinant (left-hand side of a functional dependency) must be a superkey.

**Tip**: Aim for 3NF in most designs for a good balance of integrity and performance.

Key SQL Concepts
----------------

* SQL is a Structured Query Language for communicating with relational databases.
* **Basic commands** → `SELECT`, `INSERT`, `UPDATE`, `DELETE`, `CREATE TABLE`, `ALTER TABLE`, etc.
* `Joins` → Combines data from multiple tables (`INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `FULL JOIN`).

Running SQL Commands in Bash
----------------------------

You can run SQL commands directly from the command line using the `psql` command-line client for PostgreSQL or similar tools for other databases.

For example, to run a SQL file in PostgreSQL:

```
psql -U username -d database_name -c "SELECT * FROM students;"
```

You can also execute MySQL commands directly:

```
mysql -u username -p database_name -e "SELECT * FROM students;"
```

### Run SQL from a File

```
# PostgreSQL
psql -U username -d database_name -f script.sql

# MySQL
mysql -u username -p database_name < script.sql
```

### Embed SQL in a Bash Script

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"

# Insert student data
psql -U "$DB_USER" -d "$DB_NAME" -c \
"INSERT INTO students (name, age, major) VALUES ('Alice', 20, 'CS');"
```

### Use of Variables in SQL

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"
STUDENT_NAME="Bob"
AGE=21

psql -U "$DB_USER" -d "$DB_NAME" -c \
"INSERT INTO students (name, age) VALUES ('$STUDENT_NAME', $AGE);"
```

**Tip**: Sanitize variables to avoid SQL injection.

Retrieving and Using SQL Query Results in Bash
----------------------------------------------

When you run SQL queries via `psql`, you can **capture** and **process** the returned values in your Bash scripts.

### Capturing a Single Value

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"

# Get total student count
STUDENT_COUNT=$(psql -U "$DB_USER" -d "$DB_NAME" -t -A -c \
"SELECT COUNT(*) FROM students;")

echo "Total students: $STUDENT_COUNT"
```

Output → 42

### Retrieving Multiple Columns

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"

# Get top 3 students' names and ages
RESULTS=$(psql -U "$DB_USER" -d "$DB_NAME" -t -A -F"," -c \
"SELECT name, age FROM students LIMIT 3;")

echo "Top 3 students:"
echo "$RESULTS"
```

Output

```
Alice,20
Bob,21
Charlie,22
```

### Looping Through Query Results

```
#!/bin/bash
DB_USER="school_admin"
DB_NAME="school"

# Get student names and majors
psql -U "$DB_USER" -d "$DB_NAME" -t -A -F"," -c \
"SELECT name, major FROM students;" | while IFS="," read -r name major
do
    echo "Student: $name | Major: $major"
done
```

Shape of Output

```
Student: Alice | Major: CS
Student: Bob   | Major: Math
Student: Carol | Major: Physics
```

SQL Injection
-------------

It is a web security vulnerability where attackers insert malicious SQL code into input fields to manipulate the database.

This can lead to risky actions like:

* Bypassing authentication.
* Stealing sensitive data.
* Modifying or deleting records.

An example of an SQL injection attack:

```
SELECT * FROM users WHERE username = ' " " OR "1"="1" -- ' AND password = 'anything';
```

This query would return all users because the condition `OR "1"="1"` is always true, allowing attackers to bypass login checks.

### Preventing SQL Injection

1. **Use Prepared Statements**: These separate SQL code from data, preventing injection. Here's an example (Node.js with pg):

   ```
   client.query('SELECT * FROM users WHERE username = $1 AND password = $2', [username, password]);
   ```
2. **Input Validation**: Sanitize and validate all user inputs to ensure they conform to expected formats.
3. **Least Privilege**: Use database accounts with the minimum permissions necessary for the application.

**Note**: Never grant admin rights to application accounts.

N+1 Problem
-----------

The N+1 problem occurs when an application makes one query to retrieve a list of items (N) and then makes an additional query for each item to retrieve related data, resulting in N+1 queries.

**Why It's Bad**

* Each query adds network and processing overhead.
* Multiple small queries are slower than one optimized query.

### Example of N+1 Pattern

```
-- 1: Get list of orders
SELECT * FROM orders LIMIT 50;

-- N: For each order, get customer
SELECT * FROM customers WHERE customer_id = ...;
```

**Solution**: Use `JOINs` or other set-based operations.

```
SELECT 
  orders.order_id,
  orders.product,
  orders.quantity,
  customers.customer_id,
  customers.name,
  customers.email,
  customers.address
FROM orders
JOIN customers 
  ON orders.customer_id = customers.customer_id
WHERE orders.order_id IN (SELECT order_id FROM orders LIMIT 50);
```

Always look for opportunities to combine related data into a single query.

---

