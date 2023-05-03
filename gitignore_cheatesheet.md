# Rules for .gitignore

## Pattern          Explanation/Matches                  	                               Examples
                    Blank lines are ignored
#Text comment       Lines starting with # are ignored                                                     

name                All name files, name folders and files and folders in                  /name.log
                    any name folder                                                        /name/file.txt
                                                                                           /name/lib.log
lib/name.file       Patterns specifying files in specific folders are always relative root  /lib/name.file, name.file, /test/lib/name.file
**/lib/name.file    Starting with ** before / specifies that it matches any folder in the   /lib/name.file, /test/lib/name.file
                    repository. Not just on root.
**/name             All name folders, and files and folders in any name folder               /name/log.file, 
                                                                                             /name/lib/log.file