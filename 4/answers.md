1. **Commands**
    - `uptime -p`

   **Explanation**: The `uptime` command with the `-p` (pretty) flag displays the system's up duration in a simple, easy-to-read format.

   **Output**:
   ```bash
   up 2 weeks, 1 day, 16 hours, 39 minutes
   ```

   **Screenshot**:
   ![Output](screenshot-1.png)
2. **Commands**
    - `ps -u $USER`

   **Explanation**: The `ps` command with the `-u` flag lists all active processes associated with your specific username.

   **Output**:
   ```bash
     PID TTY          TIME CMD
       1 ?        00:00:00 vnc_startup.sh
      13 ?        00:00:00 bash
      27 ?        00:00:00 python
      38 ?        00:00:07 Xvnc
      47 ?        00:00:00 sh
      56 ?        00:00:00 sh
      73 ?        00:00:00 dbus-launch
      75 ?        00:00:00 dbus-daemon
      84 ?        00:00:00 xfwm4
      96 ?        00:00:00 dbus-launch
      97 ?        00:00:00 dbus-daemon
     105 ?        00:00:02 python
     106 ?        00:00:00 ssh-agent
     119 ?        00:00:00 xfconfd
     120 ?        00:00:00 xfce4-session
     123 ?        00:00:00 xfconfd
     127 ?        00:00:00 gpg-agent
     133 ?        00:00:00 xfce4-panel
     135 ?        00:00:00 Thunar
     137 ?        00:00:00 xfdesktop
     142 ?        00:00:00 xfsettingsd
     151 ?        00:00:00 pulseaudio
     153 ?        00:00:00 gvfsd
     175 ?        00:00:00 panel-2-actions
     182 ?        00:00:00 gvfs-udisks2-vo
     189 ?        00:00:00 gvfsd-metadata
     193 ?        00:00:00 gvfsd-trash
     246 ?        00:00:00 at-spi-bus-laun
     251 ?        00:00:00 dbus-daemon
     253 ?        00:00:00 at-spi2-registr
     258 ?        00:00:01 xfce4-terminal
     262 pts/0    00:00:00 bash
     314 pts/0    00:00:00 ps
   ```

   **Screenshot**:
   ![Output](screenshot-1.png)
3. **Commands**
    - `top -u $USER`

   **Explanation**: Running `top` filtered by your user allows you to see real-time resource usage; you can press `P` to sort by the highest CPU consumption.

   **Output**:
   ```bash
   top - 14:28:33 up 15 days, 13:25,  0 users,  load average: 3.52, 3.09, 3.58
   Tasks:  34 total,   1 running,  33 sleeping,   0 stopped,   0 zombie
   %Cpu(s): 10.5 us,  3.5 sy,  0.0 ni, 85.2 id,  0.7 wa,  0.0 hi,  0.0 si,  0.0 st
   KiB Mem : 26112393+total,  7536896 free, 11742654+used, 13616049+buff/cache
   KiB Swap: 8388604 total,  6376188 free,  2012416 used, 14122638+avail Mem
   ```

   **Screenshot**:
   ![Output](screenshot-2.png)
4. **Commands**
    - `sleep 100 &`
    - `jobs`

   **Explanation**: Adding `&` to a command starts it in the background, and the `jobs` command verifies that the process is active in the background.

   **Output**:
   ```bash
   [1] 272
   [1]+  Running                 sleep 100 &
   ```

   **Screenshot**:
   ![Output](screenshot-3.png)
5. **Commands**
    - `renice +10 -p 272`

   **Explanation**: The `renice` command changes the priority (niceness) of an existing process; a higher value like `+10` gives the process lower priority, making it "nicer" to other tasks.

   **Output**:
   ```bash
   272 (process ID) old priority 0, new priority 10
   ```
   
   **Screenshot**:
   ![Output](screenshot-3.png)
6. **Commands**
    - `free -h`

   **Explanation**: The `free` command displays the total, used, and available physical and swap memory in human-readable units (e.g., GB or MB).

   **Output**:
   ```bash
                 total        used        free      shared  buff/cache   available
   Mem:           249G        113G        5.5G        177M        130G        133G
   Swap:          8.0G        1.9G        6.1G
   ```

   **Screenshot**:
   ![Output](screenshot-3.png)
7. **Commands**
    - `df -h`

   **Explanation**: Using `df -h` with a dot (`.`) targets only the filesystem associated with your current location (your home directory). Note: The screenshot shows `df -h` run globally.

   **Output**:
   ```bash
   Filesystem                                                                              Size  Used Avail Use% Mounted on
   dockerPool/d0c83627e9b7f36947aadc72413683da37e531d68e99e558f319ee7fb3710010              13G  3.7G  9.4G  29% /
   tmpfs                                                                                    64M     0   64M   0% /dev
   shm                                                                                      64M     0   64M   0% /dev/shm
   dockerPool                                                                              245G  6.8G  238G   3% /etc/hosts
   fs-096477e837a108781.efs.us-east-1.amazonaws.com:/workspaces/acbzampoaeqm/volumes/DByYRL0a/files  8.0E   85T  8.0E   1% /home/coder/Desktop
   fs-096477e837a108781.efs.us-east-1.amazonaws.com:/templates/iTq0PTcr/v1/files                     8.0E   85T  8.0E   1% /home/coder/Desktop-ro
   devtmpfs                                                                                125G     0  125G   0% /dev/tty
   tmpfs                                                                                   125G     0  125G   0% /proc/acpi
   tmpfs                                                                                   125G     0  125G   0% /proc/scsi
   tmpfs                                                                                   125G     0  125G   0% /sys/firmware
   ```

   **Screenshot**:
   ![Output](screenshot-3.png)
8. **Commands**
    - `echo $SHELL`

   **Explanation**: This command prints the value of the `$SHELL` environment variable, which stores the path to your current command-line interpreter (e.g., `/bin/bash`).

   **Output**:
   ```bash
   /bin/bash
   ```

   **Screenshot**:
   ![Output](screenshot-3.png)
9. **Commands**
    - `lscpu > system_report.txt`

   **Explanation**: This command takes the detailed CPU architecture information and uses the `>` operator to save it into a file instead of printing it to the screen.

   **Output**:
   ```bash
   ```

   **Screenshot**:
   ![Output](screenshot-3.png)
10. **Commands**
    - `ncdu ~`

   **Explanation**: `ncdu` is an interactive disk usage analyzer; it provides a visual, navigable interface to see which folders and files are consuming the most space in your home directory.