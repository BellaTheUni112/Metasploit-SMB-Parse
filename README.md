# SMB Parse


A simple parser tool for output from Metasploit's auxiliary/scanner/smb/smb_version module giving a clean report.


# How to use

Start Metasploit-Framework if not already started


```bash
msfconsole
```


inside Metasploit,



```bash
use auxiliary/scanner/smb/smb_version
set RHOSTS your ip list here or for a file it's file:yourfile.ext
set THREADS 16
spool /path/to/file.ext or file.ext idk
run
spool off
exit
```

run the tool



```bash
python metasploit-smbversion-parse.py --input file.ext
```


or for custom output



```bash
python metasploit-smbversion-parse.py --input file.ext --txt file.txt --csv file.csv
```
