# The `touch` Command

Using the `touch` command with a file name as an argument, the file will be created unless -c or -h is supplied.  If the file already exists, its modification time
will be changed.

---
### Examples
1. To make a new text file use the following command, if it does not already exist a new file will be created. Otherwise it will be overwritten.

```
touch file.txt
```
2. You can use the touch command to create multiple files. These files will be empty after creation.

```
touch File1_name File2_name File3_name 
```

---

#### **A  FILE  argument string of - is handled specially and causes touch to change the times of the file associated with standard output.**

#### Mandatory arguments to long options are mandatory for short options too.


|**Short Flag**   |**Long Flag**   |**Description**   |
|:---|:---|:---|
| `-a` | |     change only the access time |
|  `-c`| `--no-create` | do not create any files |
| `-d` |`--date=STRING`| parse STRING and use it instead of current time|
|`-f` | | (ignored) |
|`-h` | `--no-dereference` |affect each symbolic link instead of any referenced file (useful  only  on  systems that can change the timestamps of a symlink) |
|`-m` | | change only the modification time |
|`-r`|  `--reference=FILE` | use this file's times instead of current time |
|`-t STAMP` | | use [[CC]YY]MMDDhhmm[.ss] instead of current time |
| ` `  | `--time=WORD` |change  the specified time: `WORD` is access, atime, or use: equivalent to `-a WORD` is modify or `mtime`: equivalent to `-m` |
| ` ` | `--help` | display this help and exit |
| ` ` | `--version` |output version information and exit|


Note that the `-d` and `-t` options accept different time-date formats.
