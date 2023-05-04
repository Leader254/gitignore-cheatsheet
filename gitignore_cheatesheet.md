## Patterns for .gitignore Files

| Pattern            | Explanation/Matches                                                                       | Examples                                                        |
| ------------------ | ---------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
|                    | Blank lines are ignored                                                                   |                                                                 |
| `#Text comment`     | Lines starting with # are ignored                                                         |                                                                 |
| `name`             | All name files, name folders and files and folders in any name folder                     | `/name.log`, `/name/file.txt`, `/name/lib.log`                 |
| `lib/name.file`    | Patterns specifying files in specific folders are always relative root                    | `/lib/name.file`, `name.file`, `/test/lib/name.file`           |
| `**/lib/name.file` | Starting with ** before / specifies that it matches any folder in the repository         | `/lib/name.file`, `/test/lib/name.file`                        |
| `**/name`          | All name folders, and files and folders in any name folder                               | `/name/log.file`, `/name/lib/log.file`                          |
| `*.file`           | All files withe .file extention                                                          | `/name.file`, `/lib/name.file`                                 |
| `*name/`           | All folders ending with name                                                             | `/lastname/log.file`, `/firstname/log.file`                     |
| `name?.file`       | ? matches a single non-specific character                                                | `/names.file`, `/name1.file`                                   |
| `name[a-z].file`   | [range] matches a single character in the specified range (a-z and also numeric in this case) | `/names.file`, `/nameb.file` |
