## COMMANDS

- **whoami**: show user whose loged in
- **find**: finds file
	- *find -name passwords.txt* - show dir of passwords.txt
	- *find -name *.txt* - show everything that is **.txt**
- **grep**: search for content
- **wc**: return *n* of `lines, words, chars`

| Symbol / Operator | Description |
|-------------------|-------------|
| &                 | This operator allows you to run commands in the background of your terminal. |
| &&                | This operator allows you to combine multiple commands together in one line of your terminal. |
| >                 | This operator is a redirector - meaning that we can take the output from a command (such as using cat to output a file) and direct it elsewhere. |
| >>                | This operator does the same function as the `>` operator but appends the output rather than replacing (meaning nothing is overwritten). |
- **file**: determine file type
## File System
- **/etc**: system files for programs
	- passwords hashed in sha512 in *passwd, shadow*
- **/var**: store data for frequently access services *db*
- **/tmp**: it stores temp files that are used once
	- when system is restarted the tmp folder content is deleated
## File Transfer
- **wget**: downloading images from website
	- usefull for downloading big n of pictures
- **scp**: copying files between 2 computers
	- from local `scp important.txt ubuntu@192.168.1.30:/home/ubuntu/transferred.txt`
	- to local `scp ubuntu@192.168.1.30:/home/ubuntu/documents.txt notes.t`
- **python server**(`python -m http.server`): 
	- you can download files from the server with *wget* or *curl*
## Procesy
- **PID**: Id procesu
- **ps**: shows processes for the user
- **ps aux**: show process for all of the users
- **top**: it is like *aux* is it updateing every 10 seconds and it is dynamic
- **kill (PID)**: end proces
	- SIGTERM - Kill the process, but allow it to do some cleanup tasks beforehand
	- SIGKILL - Kill the process - doesn't do any cleanup after the fact
	- SIGSTOP - Stop/suspend a process

