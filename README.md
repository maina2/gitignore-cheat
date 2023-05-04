# Patterns for .gitignore files
| Pattern | Explanation/Matches | Examples |
| -------- | -------- | -------- |
| file.txt | All files with file.txt will be ignored | file.txt |
| Lines starting with a # symbol | These lines are comments and will be totally ignored by git | # this is a gitignore file|
| Blank lines | Blank lines are totally ignored by  git |  |
| *.txt | ignores all files that end with .txt extension or the specified extension | samp.txt, file1.txt, file2.txt, example.txt will all be ignored |
| logs/ | it ignores the logs directory and all of its contents (or the specified directory) | logs/, node_modules/, pycache/ |
| ** | Matches directories and their sub-directories | to ignore files with '.tmp' extension in any directory, we will use `**/*.tmp` |
| ! | includes a file or a directory that would otherwise be ignored | if file1.txt was in node_modules and node_modules folder is in gitignore but we don't want to ignore that file, we will do `!node_modules/file1.txt` This will ignore all the everything in node_modules except file1.txt |
| name[abc].file | [set] matches a single character in the specified set of characters (in this case either a, b, or c) | /namea.file, /nameb.file |