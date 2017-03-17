# AFS
*kinit user@domain* authenticates *user*; *domain* is CRC.ND.EDU or ND.EDU
*aklog domain* obtains AFS token on *domain* for authorized user
*klist* lists *Kerberos User Authentications*
*tokens* lists AFS tokens held
*unlog* destroys current AFS tokens held
*fs listquota directory* shows space used by AFS volume
*fs listacl directory* shows Access Control Lists for directory

# ssh
*ssh user@host* connect to *host* as *user*
*scp -r files user@hosr:path* copy *files* to *path* on *host* *recursively* as *user*
*ssh-copy-id user@host* add your key to *host* for *user* to enable a keyed or passwordless login

# System info.
*date* shows current date and time
*cal* shows current month/calendar
*uptime* shows current uptime
*w* displays who is online
*whoami* displays who you are logged in as
*finger user* displays infomation about a *user*
*uname -a* shows kernel information
*cat /proc/cpuinfo* shows cpu information
*cat /proc/meminfo* shows memory information
*man command* shows *command* manual
*df* shows disk usage
*du* shows directory space usage
*free* shows memory and swap usage
*whereis app* shows possible locations of *app*
*which app* shows which *app* will be run by default

# Network
*ping host* pings host and outputs results
*wget file* download *file*
*wget -c file* continue a stopped download

# Process management
*ps* display current active processes
*top* display all running processes
*kill pid* kill process id *pid*
*killall proc* kill all processes named *proc* (use this with extreme caution)
*bg* lists stopped or background jobs; resume stopped job in the background
*fg* bring most recent job to foreground
*fg n* bring job *n* to the foreground

# File permissions
*chmod octal file* change permissions of file to *octal*, which can be manuipulated for user, group and world
- *4* read(r)
- *2* write(w)
- *1* execute(x)
Examples: *chmod 777* read, write and execute for all
          *chmod 755* rwx for owner, rx for group and world
          See *man chmod* for more options

# File commands
*ls* directory listing
*ls -al* formatted listing with hidden(.) files
*cd dir* change directory to *dir*
*cd* change to home directory
*pwd* show current directory
*mkdir dir* create the directory *dir*
*rm file* delete *file*
*rm -r dir* delete directory *dir*
*rm -f file* force remove *file*
*rm -rf dir* force remove directory *dir* (use this with extreme caution)
*cp file1 /path/to/directory/file2* copy file1 to file2
*cp -r dir1 /path/to/directory/dir2* copy dir1 to dir2 (create *dir2* if it does not exist)
*mv file1 file2* rename/remove *file1* to *file2*
*ln -s file link* create symbolic link to file
*touch file* create/update *file*
*cat > file* place standard input into file
*more file* output contents of file
*head file* output first 10 lines of file
*head -n [INT] file* output first [INT] lines of file
*tail file* output last 10 lines of file
*tail -n [INT] file* output last [INT] lines of file
*tail -f file* output contents of file as it grows, starting with last 10 lines

# Compression
*tar cf file.tar files* creates tar *tar.file* containing *files*
*tar xf file.tar* extracts files from *file.tar*
*tar czf file.tar.gz files* creates tar with *gzip* compression
*tar zxf file.tar.gz files* extracts tar using *gzip*
*tar cjf file.tar.bz2* creates tar with Bzip2 compression
*tar xjf file.tar bz2* extracts tar using bzip2
*gzip file* compresses *file* and renames it to *file.gz*
*gzip -d file.gz* decompresses *file.gz* back to *file*

# Searching
*grep pattern files* search for *pattern* in *files*
*grep -r pattern dir* search *recursively* for *pattern* in *dir*
*command | grep pattern* search for *pattern* in output of *command*
*locate file* find all instances of *file*

# Shortcuts
*Ctrl+C* halts current command
*Ctrl+Z* stops current command and resumes with *fg* in foreground or *bg* in background
*Ctrl+D* logs out of current session ~*exit*
*Ctrl+W* erases one word in current line
*Ctrl+U* erases whole line
*Ctrl+R* brings up recent command
*!!* repeats last command
*exit* logs out of current session
