# Task 1 – Bash Automation for Large File Management

## Implemented
- Bash script to generate files of different sizes using OS commands
- Detection of files larger than 50MB
- Sorting files in descending order based on size

## Script
- file_management.sh

## Large File Commit & Cleanup (Design Approach)

### Committing large files
A file larger than 2GB can be committed to Git for testing purposes.

### Cleaning large files using BFG
The repository can be cleaned using BFG Repo-Cleaner:


### Cron Job (Concept)
A cron job can periodically scan for large files:
- If file size > 50MB → remove
- If file size < 50MB → commit

Example cron entry:
0 * * * * /path/to/file_management.sh


### Jenkins Job (Concept)
A Jenkins pipeline can:
- Run the bash script
- Detect large files
- Clean repository if needed
- Commit allowed files


