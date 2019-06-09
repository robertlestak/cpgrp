# cpgrp 

Group and copy files into directories based on shared file names.

## Usage

````
cpgrp source_directory target_directory
````

## Installation

The script can either be used by dropping the `cpgrp` file into the directory in question and calling locally (`./cpgrp . output`), or by placing it in your `bin` directory to be used across the system (either `/user/local/bin` or `/bin`, depending on your needs).

### Example

Given a directory `data` containing the following files:

````
foo.txt foo.md foo.xml bar.txt bar.md bar.xml
````

````
cpgrp data /tmp/output
````

Will create the following:

````
/tmp/output/foo/
	foo.txt
	foo.md
	foo.xml
/tmp/output/bar/
	bar.txt
	bar.md
	bar.xml
````
