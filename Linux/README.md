# Linux

## Transferring files from local to AFS
*scp* < file > *rwiltshi@opteron.crc.nd.edu***:***/afs/crc.nd.edu/user/r/rwiltshi/< rest of PATH >*

Opteron may change depending on which machine you are logged into i.e. darrow, phillips etc.

## If you lose your bash commands because of an incorrectly set PATH
Call the absolute path to the command i.e. ***/usr/bin/nano ~/.bashrc*** and then edit accordingly

Put this in your $PATH i.e. ***PATH=/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin:/usr/X11/bin***

## FTP transfers
This took forever on the NCBI website - ever heard of comments? To upload files via ftp:
- *cd* to the directory on **afs space where the files are located** and type your ftp command: 
  - *ftp* ftp-private.ncbi.nlm.nih.gov
  - name: *sra*
  - password: (whatever they give you)
- create directory on ftp space to move the files:
  - *mkdir* PRJNAXXXXXX
- *cd* to the new directory:
  - *cd* PRJNAXXXXXX
- effect the transfer:
  - *mput* < file >
  
### Useful FTP commands
  - *prompt* > toggles interactive on/off
  - *put* > transfers one file
  - *mput* > transfers multiple files
  - *user* > changes user log in

## To view binary files
*xxd -b* file.bed

## To create a symbolic link
*ln -s* /path-to-shortcut

## To move the cursor in the line
- control + a (beginning)

- control + e (end)

## To append output to a file
*command >>* < newfile.whatever >

## To print a sequence of numbers 

- *seq LAST*
  [default is 1 so unless you are specifying a sequence that doesn't start at 1 it is sufficient to enter the final number]
- *seq FIRST LAST*
- *seq FIRST INCREMENT LAST* 
  [if the sequence is not sequential by one integer i.e seq 2 2 20 will return 2 4 6 8 10 12 14 16 18 20]
- *seq LAST | cat >* < file.xtn >
  [writes the sequence output to a file]

## To return a column/field from a file
*cut -f***[INT]**

## To combine two or more files line by line
*paste* < file.xtn > < file.xtn > **>** < outputfile.xtn > [pipes to standard out if no outfile specified]

## screen
OMG this is the *most* useful command I've found whilst attempting to run long jobs. ***screen*** allows the user to execute multiple programs without interrupting the command.

All commands must begin with ***control + a*** to distinguish ***screen*** from the normal shell followed by one of:

- *control + c* - **c**reates a new screen to allow multiple sessions

- *control + d* - **d**etaches screen session

- *control + n* - switches to **n**ext screen session (if more than one session is running)

- *control + p* - switches to **p**revious screen session (if more than one session is running)

- *control + r* < session > - **r**econnects to a screen session

Help can be found here > *man screen*

###Usage

  1) Command line prompt > *screen*

  2) Execute program

  3) *control a d* to detach the session from the normal shell
  
  4) In the normal shell you can list all your active sessions by typing: *screen -ls*
  
  5) To leave and finish a session -> *exit*
