# FileStripper

## Command invocation format: 
    ./FileStripper uploadFile downloadFile
## Prerequisites:
    The two files being compared MUST be in the same directory as the executable
        OR
    The full path of the files MUST be provided in the arguments of the command invocation
## Inputs:
    uploadFile path
    downloadFile path
## Outputs:
    newFile (written into directory of the program's executable)
## Function Information:
    FileStripper strips the filler bytes from the end of downloaded binary files, 
    compares the resulting new file to the original upload file via SHA-256 hash comparison,
    and verifies the validity of the new file.
    
    All arguments are mandatory.
## To-Do:
    1. Get rid of stripped file (downloadFile) - do comparison using system() command
