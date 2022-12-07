# OSCE

-------------------------------------\_~~__(··)_~~_/-------------------------------------------

This repository contains a script that i had used to identity bad characters when developing buffer overflow scripts for old OSCE

Badcharacter Detection:

  -Takes a bad character  and see which character breaks / terminates the string
  -Loops from 0x00 - 0xff
  -The application to test has to be on the same host
  -Written for HTTP . With minor modifaction this can be made to work with FTP / Telnet

- [Certify](#certify)
  - [Usage](#usage)
    - [Using Requested Certificates](#using-requested-certificates)
  - [Example Walkthrough](#example-walkthrough)
  - [Defensive Considerations](#defensive-considerations)
  - [Compile Instructions](#compile-instructions)
    - [Sidenote: Running Certify Through PowerShell](#sidenote-running-certify-through-powershell)
      - [Sidenote Sidenote: Running Certify Over PSRemoting](#sidenote-sidenote-running-certify-over-psremoting)
  - [Reflections](#reflections)
  - [Acknowledgments](#acknowledgments)
