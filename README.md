# OSCE

-------------------------------------\_~~__(··)_~~_/-------------------------------------------

This repository contains a script that i had used to identity bad characters when developing buffer overflow scripts for old OSCE

Badcharacter Detection:

  -Takes a bad character  and see which character breaks / terminates the string
  -Loops from 0x00 - 0xff
  -The application to test has to be on the same host
  -Written for HTTP . With minor modifaction this can be made to work with FTP / Telnet
