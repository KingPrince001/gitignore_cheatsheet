| Pattern | Explanation | Example |
|---------|-------------|---------|
| `*` | Matches any string of characters, except for `/` | `*.txt` matches all `.txt` files in a directory |
| `?` | Matches any single character, except for `/` | `file?.txt` matches `file1.txt`, `file2.txt`, but not `file11.txt` |
| `**` | Matches any string of characters, including `/` | `dir/**/file.txt` matches `dir/file.txt`, `dir/subdir/file.txt`, etc. |
| `{}` | Matches any of the comma-separated patterns inside the braces | `{*.jpg,*.png}` matches all `.jpg` and `.png` files |
| `!` | Negates a pattern (i.e., matches anything that does not match the pattern) | `!*.txt` matches all files that are not `.txt` |
| `/` | Matches the directory separator (e.g., `/` on Unix) | `/dir/subdir/file.txt` matches `file.txt` only if it's inside `subdir`, not in other subdirectories |
| `#` | Indicates a comment (not a pattern) | `# This is a comment` |
| ` ` | Empty space is ignored (useful for aligning patterns) | `*.{txt,jpg}` and `*.png` are equivalent |