By Jacob Zaidi.

This program must be run from the command line with a Linux distribution. It implements a user space file system which automatically keeps multiple versions of files, and implements tools to work with the file versions.

The following command creates a directory called .versiondir. Any files created in mount will be created in .versiondir.
python versionfs.py mount 

Using another terminal, create and edit files in the mount directory. These files will be created in the .versiondir directory with a version number, from one to six.

