# OSCE

-------------------------------------\_~~__(··)_~~_/-------------------------------------------

This repository contains a script that i had used to identity bad characters when developing buffer overflow scripts for old OSCE



- Badcharacter Detection:
  - Takes a bad character  and see which character breaks / terminates the string.
  - Loops from 0x00 - 0xff.
  - The application to test has to be on the same host.
  - Written for HTTP . With minor modifaction this can be made to work with FTP / Telnet.

- How to make it work:
  - Modify the template to match the requirement (HTTP /FTP). In the poc , HTTP is choosen and UserID={} in Cookie Header will be fuzzed.
  - modify the script to change the desired process to hook for. Note that the service must able to start and stop with sc.exe (start / stop).
  - Every chacrater wil be fuzzed in the format - "A"*8 + cur_char * 92 + "B"*8 (eg for 0x00 - 4141414141414141 + 00*92 + 4242424242424242.
  - The process will be killed and restarted multiple times for looping badcharacters from 0x00 - 0xff.
