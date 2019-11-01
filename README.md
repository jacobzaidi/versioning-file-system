## About Versioning File System

Versioning File System implements a user space file system which automatically keeps multiple versions of files, and implements tools to work with the file versions. The project is compatible with a Linux distribution and not Windows or MacOS.

## Instructions for how to develop, use, and test the code.

You may use either the Python or Bash folder to use the code.

1. You will need two terminal windows open: one to run the user space file system and display the output, and one to work with files from the command line.

2. In terminal one create a directory called mount. Then run the program: `python versionfs.py mount`.

3. From here on all commands should be executed in terminal two.

## What functions can I call 

* `listversions filename` lists the versions of the file called `filename`.

* `mkcurrent filename version#` makes `version#` the current version of the file `filename`.

* `catversion filename version#` displays the contents of the version `version#` of the file `filename` on the screen.
 
* `rmversions filename` permanently removes all versions except the current version of file `filename`.

* `shutdownversions` removes all files and cleans out all directories created by the versioning file system.

## Credits

* `fuse.py` originally came from [fuse.py](https://github.com/fusepy/fusepy)

* `versionfs.py` is based on [passthrough.py](https://github.com/skorokithakis/pythonfuse-sample)

