# libs
Collection of Bash functions, scripts and programs for use on their own or as source files within other Bash scripts.

# Collection
Public collection currently includes:

- softman: wrapper for frequently used apt-get command line sequences, plus a few bonus tools.
- parseconf: file parser that looks for key=value lines in files. Values are loaded into an associative array. Useful for parsing config files.

# Organization
Each file is filtered into 1 of 3 directories depending on what it does:

- 0: Each file is a solo function. Useful code snippets.
- 1: Each file is a self-contained script made mostly of functions within directory 0.
- 2: Each file is dependent on scripts within either/both directories 0 and/or 1.

There is also a directory for examples:

- examples: these demonstrate how to use the library of scripts.

# Features

## Files in directory 0
- Base functions. These are effectively useful Bash code snippets. These are used within the more useful scripts in directories 1 and 2.

## Files in directory 1
- All scripts ship with help text. Access with the -h flag.
- All scripts ship with a version number. Access with the -v flag.
- All scripts can execute when clicked in a GUI environment provided the file is made executable.
- All scripts can be loaded into a parent script (as a source file) with options/arguments passed to the script. See each script's help text for details.

## Files in directory 2
- These are unifying scripts. These combine features of scripts within directories 0 and 1 to perform complex tasks.

## Usage

Generally speaking,

- Copy and paste the snippets of directory 0 into your own scripts. See scripts in director 1 for examples.
- Use scripts in directory 1 as you would any other Bash script e.g. Make the file executable and run with ./script-name or just click the file to run its default task. You can also use these within other scripts.
- Currently, to use scripts in directory 2 you will need to download the whole library.

# License

GNU General Public License v3.0

See license document for details.

All scripts authored by Lee Hodson of JournalXtra.com and vr51.com.

Make sure to keep copyright notices and annotations within the scripts you use.

If you find the scripts useful and can afford to contribute finanically to development send contributions to https://paypal.me/vr51
