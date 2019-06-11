# Useful Linux Commands

It will be helpful to know some linux commands this summer while working on your projects. Some of the most useful ones are given below and grouped by their use case.

`talk about opening terminal and what is displayed at the prompt ie username current folder $`

## Documentation

* talk about the man pages and --help

## Disk Space and Usage

Display human-readable (-h) free disk space:
```
!df -h
```
Display human-readable (-h) disk usage statistics:
```
!du -h ./
```
Display human-readable (-h) disk usage statistics, showing only the total usage (-s):
```
!du -sh ../
```
Display the human-readable (-h) disk usage statistics, showing also the grand total for all file types (-c):
```
!du -csh ./
```

## File and Folder Manipulation

* need to add cat, more, touch, cd, mkdir, cp, rm (warning)

Count number of lines in a file with wc:
```
!wc -l < file.txt
```
Count the number of lines in a file with grep:
```
!grep -c "." file.txt
```
Split a file into multiple files based on line count:
```
!split -l 20 file.txt new
```
Split a file into multiple files based on line count, use suffix of length 1:
```
!split -l 802 -a 1 file.csv dir/part-user-csv.tbl-
```

## Grep and Find

List number of files matching “.txt":
```
!ls -1 | grep .txt | wc -l
```
Check number of MapReduce records processed, outputting the results to the terminal:
```
!cat * | grep -c "foo" folder/part*
```
Delete matching lines in place:
```
!sed -i '/Important Lines: /d’ original_file
```

## Compression

```
# Compress zip
!zip -r archive_name.zip folder_to_compress

# Compress zip without invisible Mac resources
!zip -r -X archive_name.zip folder_to_compress

# Extract zip
!unzip archive_name.zip

# Compress TAR.GZ
!tar -zcvf archive_name.tar.gz folder_to_compress

# Extract TAR.GZ
!tar -zxvf archive_name.tar.gz

# Compress TAR.BZ2
!tar -jcvf archive_name.tar.bz2 folder_to_compress

# Extract TAR.BZ2
!tar -jxvf archive_name.tar.bz2

# Extract GZ
!gunzip archivename.gz

# Uncompress all tar.gz in current directory to another directory
!for i in *.tar.gz; do echo working on $i; tar xvzf $i -C directory/ ; done
```

## Piping

* add in | < >
```
| > <
```

## View Running Processes

```
# Display sorted info about processes
!htop

# Display all running processes
!ps aux | less

# Display all matching running processes with full formatting
!ps -ef | grep python

# See processes run by user dmartin
!ps -u dmartin

# Display running processes as a tree
!pstree
```

## Exiting Vim

If you somehow end up in vim, the command to exit press `esc` many times then enter `:q` or `:!q` . If you want to save any changes that have been made enter `:wq`.
