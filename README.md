# Bug-Fix
Fixed bugs

-----------------------------------------------

## Issue
Jupyter Notebook not working [RESOLVED]
## Expected Behaviour
Click run for Notebook with 1 cell with print("hi"), and cell outputs hi
## Result
dll not found
## Cause
download sqlite.dll missing
## Method of Discovery
- Click log on popup aout kernel couldn't find dll
- Go through OUTPUT which opens
- Find sqlite
## Source
- [Unable to import sqlite3 using Anaconda Python](https://stackoverflow.com/questions/54876404/unable-to-import-sqlite3-using-anaconda-python)
## Fix
go to:
### site:
- [sqlite](https://www.sqlite.org/download.html)

#### heading:
<b><u>Precompiled Binaries for Windows</u></b>
- click download link
- [sqlite-dll-win64-x64-3410200.zip](https://www.sqlite.org/2023/sqlite-dll-win64-x64-3410200.zip)
- download
- extract

### open Windows Explorer:
C:\Users\YOURUSER\Anaconda3\DLLs

### drag file from extracted folder to Anaconda3\DLLs folder

## Test
- VSCode
- Ctrl + Shift + P
- Create Jupyter Notebook
- Add ``print("hi")`
- Click Play button Run All

## [RESOLVED]

-----------------------------------------------
