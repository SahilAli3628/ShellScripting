# Bash Commands Practice Questions | Intermediate Level

1. Query the Domain Name System for **Udemy.com**
    ```bash
    dig udemy.com
    ```
    > DIG stands for Domain Information Groper, This command is used to retrieve information about DNS name servers.

2. Identify the location of executable **bash**
    ```bash
    which bash
    ```

3. List all running processes with full format listing for each process
    ```bash
    ps aux
    ```

4. Display what programs are currently running on the system and how much system resoruces they are utilizing
    ```bash
    htop
    ```
    > you can use _top_ as well. I personally prefer _htop_

5. Which command is used to download/upload data to a server with supported protocoles such as HTTP, FTP, SFTP, IMAP, POP3, etc
    ```bash
    curl <url/fqdn>
    ```

6. Retrieve content from web [**udemy.com**](https://www.udemy.com/) into index.html file
    ```bash
    wget udemy.com
    ```

7. Search **Git** package for Linux machine
    ```bash
    <package_manager> search git
    ```
    > Except for Arch-Based systems or if you are using snap (_not sure who in their right mind would_). 
    >
    > If you are using arch, use `pacman -Ss git`
    >
    > If you are using snap, use `snap find git`

8. Print information about your linux system like the machine name and operating system
    ```bash
    fastfetch
    ```
    > You can use **uname -a** for printing the name and a few details about the machine. But **fastfetch** prints all the details properly in a user friendly manner

9. Display the status of TCP and UDP endpoints, routing table info and interface information
    ```bash
    netstat
    ```

10. Display the disk space used in the file system
    ```bash
    df
    ```

11. Display the disk space used in the file system in the Human-Readable format
    ```bash
    df -h
    ```

12. Print the network interface configuration information on screen
    ```bash
    ifconfig
    ```

13. Display details about block devices on your linux machine
    ```bash
    lsblk
    ```

14. Print the message buffer of the kernel on your linux OS
    ```bash
    dmesg
    ```

15. Create a new user name as **devops** on linux
    ```bash
    adduser devops
    ```

16. Delete the user **devops** from your machine
    ```bash
    userdel devops
    ```

17. Install a new package **httpd** on your machine
    ```bash
    sudo <package_manager> install httpd -y
    ```
    > Except for Arch-Based systems 
    >
    > If you are using arch, use `pacman -S apache`

18. Remove package **httpd** from your machine
    ```bash
    sudo <package_manager> remove httpd -y
    ```
    > Except for Arch-Based systems and Flatpak
    >
    > If you are using arch, use `pacman -R apache`
    > 
    > If you are using Flatpak, use `flatpak uninstall httpd`

19. Put your terminal on sleep for 30 seconds
    ```bash
    sleep 30
    ```

20. List all the files under **/etc** directory which are modified in the last 30 days
    ```bash
    find /etc -iname "*" -type f -mtime -30
    ```

21. Grep **root** keyword from **/var/log/dnf5.log** file
    ```bash
    grep -i "root" /var/log/dnf5.log
    ```
    > You can also use `cat /var/log/dnf5.log | grep root` but this adds an unwanted extra step

22. Print the count (# of times, root keyword found) by performing grep "**root** keyword from **/var/log/dnf5.log** file
    ```bash
    grep -ic "root" /var/log/dnf5.log 
    ```

23. Follow the below steps:
    - Create an empty file **devops.txt**
    - echo "Test" > devops.txt
    replace the **Test** word with **Hello** and update the same file using suitable command
    ```bash
    echo "Hello" > devops.txt
    ```
    > You can also use sed command here `sed -i "s/Test/Hello/" devops.txt`

24. Print Second Column of top 100 rows from **/var/log/dnf5.log** file
    ```bash
    head -100 /var/log/dnf5.log | awk '{print $2}'
    ```

25. Print Second and third Column from **/var/log/dnf5.log** file, print only for top 50 rows
    ```bash
    head -50 /var/log/dnf5.log | awk '{print $2,$3}'
    ```

