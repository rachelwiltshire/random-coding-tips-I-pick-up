# Random-coding-tips-I-pick-up
Finally, somewhere sensible to keep these rather than the post-its on my monitors!

## Linux

### If you lose your bash commands because of an incorrectly set PATH
Call the absolute path to the command i.e. **/usr/bin/nano ~/.bashrc** and then edit accordingly

Put this in your $PATH i.e. **PATH=/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin:/usr/X11/bin**

### FTP transfers
This took forever on the NCBI website - ever heard of comments? To upload files via ftp:
- *cd* to the directory on **afs space where the files are located** and type your ftp command: 
  - ftp ftp-private.ncbi.nlm.nih.gov
  - name: sra
  - password: (whatever they give you)
- create directory on ftp space to move the files:
  - *mkdir* PRJNAXXXXXX
- *cd* to the new directory:
  - *cd* PRJNAXXXXXX
- effect the transfer:
  - *mput* < file >
  
#### Useful FTP commands
  - *prompt* > toggles interactive on/off
  - *put* > transfers one file
  - *mput* > transfers multiple files
  - *user* > changes user log in

### To view binary files
xxd -b file.bed

### To create a symbolic link
ln -s /path-to-shortcut

### To move the cursor in the line
- control + a (beginning)

- control + e (end)

### To append output to a file
command >> newfile.whatever

## R

### To remove rows and columns from a matrix
I hit this problem frequently when attempting to level out my geographical and Fst matrices for Isolation By Distance regression
data

<- data[-(R:R),-(C:C)] or [-R:-R,-C:-C]
