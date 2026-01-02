1. Commands
    - `mkdir ~/documents`
   Explanation: `mkdir` (make directory) creates a new folder named `documents` in your home directory (represented by `~`).
2. Commands
    - `cd ~/documents`
    - `touch plan.txt`
   Explanation: `cd` changes the working directory to the new `documents` folder, and `touch` creates an empty file named `plan.txt`.
3. Commands
    - `echo "Project Alpha: Phase 1 starts on Monday." > plan.txt`
   Explanation: The `echo` command writes the specified string, and the `>` operator redirects that text into `plan.txt`, populating the file with content.
4. Commands
    - `ls -l plan.txt`
   Explanation: The `ls` command with the `-l` (long format) flag displays the file's permissions, owner (your username), group, and size.
5. Commands
    - `cp plan.txt plan_copy.txt`
   Explanation: The `cp` (copy) command creates a duplicate of `plan.txt` and names the new file `plan_copy.txt`.
6. Commands
    - `cd ..`
    - `mv documents project_documents`
   Explanation: After moving up one level, the `mv` (move/rename) command changes the directory name from `documents` to `project_documents`.
7. Commands
    - `mkdir project_documents/archive`
   Explanation: This command creates a new subdirectory named `archive` specifically inside the `project_documents` folder.
8. Commands
    - `mv project_documents/plan_copy.txt project_documents/archive/`
   Explanation: The `mv` command is used here to move `plan_copy.txt` from its current location into the `archive` subdirectory.
9. Commands
    - `ls -R project_documents`
   Explanation: The `ls` command with the `-R` (recursive) flag lists the contents of the directory and all its subdirectories, showing the full structure.
10. Commands
    - `realpath project_documents/archive/plan_copy.txt`
   Explanation: The `realpath` command resolves the full absolute path from the root directory (`/`) to the specific file.