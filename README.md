# LINUX COMMANDS 

### *Made by Subham Kundu* :smile: ###

| Command                                           |                  Description |
| :------------------------------------------------ | ---------------------------: |
| [file](https://www.javatpoint.com/linux-file)     |        Determines file type. |
| [touch](https://www.javatpoint.com/linux-touch)   |       Used to create a file. |
| [rm](https://www.javatpoint.com/linux-rm)         |            To remove a file. |
| [cp](https://www.javatpoint.com/linux-cp)         |              To copy a file. |
| [mv](https://www.javatpoint.com/linux-mv)         | To rename or to move a file. |
| [rename](https://www.javatpoint.com/linux-rename) |              To rename file. |



## LINUX DIRECTORY COMMANDS

| Directory Command                               |                                                  Description |
| :---------------------------------------------- | -----------------------------------------------------------: |
| [pwd](https://www.javatpoint.com/linux-pwd)     | The pwd command stands for (print working directory). It displays the current working location or directory of the user. It displays the whole working path starting with /. It is a built-in command. |
| [ls](https://www.javatpoint.com/linux-ls)       | The ls command is used to show the list of a folder. It will list out all the files in the directed folder. |
| [cd](https://www.javatpoint.com/linux-cd)       | The cd command stands for (change directory). It is used to change to the directory you want to work from the present directory. |
| [mkdir](https://www.javatpoint.com/linux-mkdir) |        With mkdir command you can create your own directory. |
| [rmdir](https://www.javatpoint.com/linux-rmdir) | The rmdir command is used to remove a directory from your system. |



## LINUX FILE CONTENTS COMMAND

| Commands                                      |                                                     Function |
| :-------------------------------------------- | -----------------------------------------------------------: |
| [head](https://www.javatpoint.com/linux-head) |                         It displays the beginning of a file. |
| [tail](https://www.javatpoint.com/linux-tail) |                    It displays the last last part of a file. |
| [cat](https://www.javatpoint.com/linux-cat)   |                  This command is versatile and multi worker. |
| [tac](https://www.javatpoint.com/linux-tac)   |                                             Opposite of cat. |
| [more](https://www.javatpoint.com/linux-more) | Command line displays contents in pager form that is either in more format. |
| [less](https://www.javatpoint.com/linux-less) | Command line displays contents in pager form that is either in less format. |

## LINUX FILTER COMMANDS

### CAT

When cat command is used inside pipes, it does nothing except moving stdin to stout.

1. Display Contents of a file:

   ```bash
   # cat /etc/passwd
   
   ```

2. View contents of multiple files

   In below example, it will display contents of **test** and **test1** file in terminal.

   ```shell
   # cat test test1
   ```

3. Create a file with Cat command

   ```shell
   # cat >test2
   ```

4. Cat command with more or less Options

   We can use it to view contents when there are many in a file and it won't fit the screen.

   ```shell
   # cat abc.txt | more
   # cat abc.txt | less
   ```

5. Cat command can be used to display the line numbers and the content both.

   

   ```shell
   # cat -n abc.txt
   ```

6. We can see with **-e** option that ‘**$**‘ is shows at the end of line and also in space showing ‘**$**‘ if there is any gap between paragraphs. This options is useful to squeeze multiple lines in a single line.

   ```shell
   # cat -e test
   
   hello everyone, how do you do?$
   $
   Hey, am fine.$
   How's your training going on?$
   $
   ```

7. Display Tab separate lines in a file with '^I'

   ```powershell
   # cat -T test
   
   hello ^Ieveryone, how do you do?
   ```

8. Standard output with redirection operator -> The output of one file can be stored in the second file.

   *** Note: The contents in the second file will be overwritten whenever this command is used.**

   

   ```shell
   # cat test > test1
   ```

9. Appending Standard output with redirection operator

   ```shell
   # cat test >> test1
   ```

10. Redirecting standard input with redirection operator

    When you use the redirect with standard input ‘**<**‘ (less than symbol), it use file name **test2** as a input for a command and output will be shown in a terminal.

    ```shell
    # cat < test2
    
    This is test2 file.
    ```

11. Redirecting multiple files in a single file

    ```shell
    # cat test test1 test2 > test3
    ```

## LINUX NETWORKING COMMANDS

| Command                                                      |                                                   FUNCTION |
| :----------------------------------------------------------- | ---------------------------------------------------------: |
| ifconfig                                                     |        Display and Manipulate Route and Network Interfaces |
| [ip](https://www.javatpoint.com/linux-ip)                    |                   It is a replacement of ifconfig command. |
| [traceroute](https://www.javatpoint.com/linux-traceroute)    |                           Network troubleshooting utility. |
| [tracepath](https://www.javatpoint.com/linux-tracepath)      | Similar to traceroute but doesn't require root privileges. |
| [ping](https://www.javatpoint.com/linux-ping)                |                   To check connectivity between two nodes. |
| [netstat](https://www.javatpoint.com/linux-netstat)          |                            Display connection information. |
| [ss](https://www.javatpoint.com/linux-ss)                    |                            It is a replacement of netstat. |
| [dig](https://www.javatpoint.com/linux-dig)                  |                             Query DNS related information. |
| [nslookup](https://www.javatpoint.com/linux-nslookup)        |                                    Find DNS related query. |
| [route](https://www.javatpoint.com/linux-route)              |                     Shows and manipulate IP routing table. |
| [host](https://www.javatpoint.com/linux-host)                |                                      Performs DNS lookups. |
| [arp](https://www.javatpoint.com/linux-arp)                  |            View or add contents of the kernel's ARP table. |
| [iwconfig](https://www.javatpoint.com/linux-iwconfig)        |              Used to configure wireless network interface. |
| [hostname](https://www.javatpoint.com/linux-hostname)        |                                To identify a network name. |
| [curl or wget](https://www.javatpoint.com/linux-curl-and-wget) |                          To download a file from internet. |
| [mtr](https://www.javatpoint.com/linux-mtr)                  |         Combines ping and tracepath into a single command. |
| [whois](https://www.javatpoint.com/linux-whois)              |                   Will tell you about the website's whois. |
| [ifplugstatus](https://www.javatpoint.com/linux-ifplugstatus) |                Tells whether a cable is plugged in or not. |



These commands are fine to start with Linux but along with these we should have some basic UNIX tools 

1. find: The find command helps us to find a particular file within a directory. It is used to find the list of files for the various conditions like permission, user ownership, modification, date/time, size, and more.

   We can do the following task using this file command

   - [Find files by name](https://www.javatpoint.com/linux-find#name)

   - [Find files by type](https://www.javatpoint.com/linux-find#type)

   - [Find newer files](https://www.javatpoint.com/linux-find#newer)

   - [Find and delete a file](https://www.javatpoint.com/linux-find#delete)

   - [Find a directory](https://www.javatpoint.com/linux-find#directory)

   - [Find files by modification time](https://www.javatpoint.com/linux-find#modification)

   - [Find files by permission](https://www.javatpoint.com/linux-find#permission)

   - [Find and replace files](https://www.javatpoint.com/linux-find#replace)

   - [Find text within multiple files](https://www.javatpoint.com/linux-find#multiple)

     

2. locate:   The locate command and [find ](https://www.javatpoint.com/linux-find)command is used to search a file by name. But, the difference between both commands is that locate command is a background process and searches the file in the database whereas, find command searches in the filesystem. The locate command is much faster than find command.

   

   `locate [OPTION]...PATTERN`

   #### Some of the well known options are:

   **-A, --all:** It is used to display only entries that match all PATTERNs instead of requiring only one of them to match.

   **-b, --basename:** It is used to match only the base name against the specified patterns.

   **-c, --count:** It is used for writing the number matching entries instead of writing file names on standard output.

   **-d, --database DBPATH:** It is used to replace the default database with DBPATH.

   **-e, --existing:** It is used to display only entries that refer to existing files during the command is executed.

   **-L, --follow:** If the '--existing' option is specified, It is used for checking whether files exist and follow trailing symbolic links. It will omit the broken symbolic links to the output. This is the default behavior. The opposite behavior can be specified using the "--nofollow" option.

   **-h, --help:** it is used to display the help documentation that contains a summary of the available options.

   **-i, --ignore-case:** It is used to ignore case sensitivity of the specified patterns.

   **-p, --ignore-spaces:** It is used to ignore punctuation and spaces when matching patterns.

   **-t, --transliterate:** It is used to ignore accents using iconv transliteration when matching patterns.

   **-l, --limit, -n LIMIT:** If this option is specified, the command exit successfully after finding LIMIT entries.

   **-m, --mmap:** It is used to ignore the compatibility with BSD, and GNU locate.

   **-0, --null:** It is used to separate the entries on output using the ASCII NUL character instead of writing each entry on a separate line.

   **-S, --statistics:** It is used to write statistics about each read database to standard output instead of searching for files.

   **-r, --regexp REGEXP:** It is used for searching a basic regexp REGEXP.

   **--regex:** It is used to describe all PATTERNs as extended regular expressions.

   **-V, --version:** It is used to display the version and license information.

   **-w, --wholename:** It is used for matching only the whole path name in specified patterns.

   

3. date:  Linux date command is used to display date, time, time zone, etc. It is also used to set the date and time of the Linux system. Generally, it is used to display the date in different formats and calculate dates over time.

4. sleep: Linux sleep command lets the terminal wait by the specified amount of time. By default, it takes time in seconds. But, we can set the delay time in minutes (m), hours (h), and days (d). It helps in pausing the execution of any particular command for a fixed amount of time.

5. zcat: Compressed files can be viewed using these command

6. bzip2: The command bzip2 is also used to compress a file like gzip command but takes a little more time but compresses better. Its extension will be **(.bz2)**. <bzip2 filename>

7. bzcat: The command bzcat will display the files compressed with bzip command.

   Syntax:

   <bzcat filename>

   ### LINUX REGUX EXPRESSION

   Regular expression is also called **regex or regexp**. It is a very powerful tool in Linux. Regular expression is a pattern for a matching string that follows some pattern.

   Regex can be used in a variety of programs like grep, sed, vi, bash, rename and many more.

   For more follow this link: https://www.javatpoint.com/linux-regular-expression

   

   

   

   

   
