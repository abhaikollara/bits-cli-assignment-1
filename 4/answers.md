1. Commands
    - `uptime -p`
   Explanation: The `uptime` command with the `-p` (pretty) flag displays the system's up duration in a simple, easy-to-read format.
2. Commands
    - `ps -u $USER`
   Explanation: The `ps` command with the `-u` flag lists all active processes associated with your specific username.
3. Commands
    - `top -u $USER`
   Explanation: Running `top` filtered by your user allows you to see real-time resource usage; you can press `P` to sort by the highest CPU consumption.
4. Commands
    - `sleep 100 &`
    - `jobs`
   Explanation: Adding `&` to a command starts it in the background, and the `jobs` command verifies that the process is active in the background.
5. Commands
    - `renice +10 -p [PID]`
   Explanation: The `renice` command changes the priority (niceness) of an existing process; a higher value like `+10` gives the process lower priority, making it "nicer" to other tasks.
6. Commands
    - `free -h`
   Explanation: The `free` command displays the total, used, and available physical and swap memory in human-readable units (e.g., GB or MB).
7. Commands
    - `df -h .`
   Explanation: Using `df -h` with a dot (`.`) targets only the filesystem associated with your current location (your home directory).
8. Commands
    - `echo $SHELL`
   Explanation: This command prints the value of the `$SHELL` environment variable, which stores the path to your current command-line interpreter (e.g., `/bin/bash`).
9. Commands
    - `lscpu > system_report.txt`
   Explanation: This command takes the detailed CPU architecture information and uses the `>` operator to save it into a file instead of printing it to the screen.
10. Commands
    - `ncdu ~`
   Explanation: `ncdu` is an interactive disk usage analyzer; it provides a visual, navigable interface to see which folders and files are consuming the most space in your home directory.