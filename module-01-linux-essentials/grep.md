📘 grep Command in Linux
grep (Global Regular Expression Print) is used to search for text patterns inside files, outputs, or streams. It’s one of the most frequently used commands for system admins, developers, and anyone using the CLI.

🔥 Basic Syntax

grep [options] pattern [file...]


📌 Most Common and Useful grep Commands

Usage	                             Command	                              Explanation
Simple search	                     grep "hello" file.txt	                Search for "hello" inside file.txt.
Case-insensitive search	           grep -i "hello" file.txt	              Ignore case (matches "hello", "HELLO", "HeLLo").
Recursive search	                 grep -r "hello" /path/to/directory	    Search through all files in a directory and its subdirectories.
Show line numbers	                 grep -n "hello" file.txt	              Show matching line numbers.
Search exact word match	           grep -w "hello" file.txt	              Only match the whole word "hello" (not "hello123").
Count matches	                     grep -c "hello" file.txt	              Count how many lines match.
Invert match	                     grep -v "hello" file.txt	              Show all lines that do not contain "hello".
Display filenames only	           grep -l "hello" *.txt	                Show only filenames with at least one match.
Search multiple patterns	         `grep -E "hello	                      world" file.txt`
Highlight matches	                 grep --color=auto "hello" file.txt	    Highlight the match in color (usually default behavior on many distros).


🎯 Frequently Combined with Other Commands

Usage	                               Command	                              Explanation
Search inside ps output	             `ps aux | grep nginx`
Find errors in logs	                 grep -i "error" /var/log/syslog	      Search for "error" messages in system logs.
Combine with dmesg	                `dmesg grep usb`
Find open ports	                    `netstat -tulnp | grep 80`


🛠️ Pro Tip: Use grep with find
If you want to search text across a large number of files:

find /path -name "*.log" | xargs grep "fatal"

Or better (handling spaces in filenames):

find /path -name "*.log" -print0 | xargs -0 grep "fatal"


🚀 Advanced Useful Flags

Flag	          Description
-A NUM	        Show NUM lines After the match.
-B NUM	        Show NUM lines Before the match.
-C NUM	        Show NUM lines Around the match (Context).
-P	            Interpret the pattern as Perl-compatible regex (PCRE).
-F	            Interpret pattern as a fixed string, not a regex (faster).

Example:

grep -C 3 "error" /var/log/syslog
Shows 3 lines before and after every match of "error."

🧠 Short Summary
grep is your go-to tool to find text fast.
It is simple yet very powerful when combined with pipelines (|), find, awk, sed, etc.
It's one of the "must-master" commands for Linux work, scripting, troubleshooting, and log analysis.
