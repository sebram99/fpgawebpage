# Utilites

## Remove file or folder tracking from git repo

Sometimes I want to remove files from version control, but I don't want to add them to `.gitignore`, 
because they are a local configuration file, so I edit exclude file in `.git/info/exclude`,
and just add the files or folder that I don't want to track in git.

    # git ls-files --others --exclude-from=.git/info/exclude
    # Lines that start with '#' are comments.
    # For a project mostly in C, the following would be a good set of
    # exclude patterns (uncomment them if you want to use them):
    # *.[oa]
    # *~
    somefile.txt
    /somedirectory

##  VSCode useful extensions

*   `vhdl_ls` Linting and syntax correction. (Note: needs `vhdl_ls.toml` file in root directory.) 
        [vhdl_ls repository](https://github.com/VHDL-LS/rust_hdl_vscode)

*   `vhdl_whiz` autocompletion.