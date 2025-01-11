# Bash Commands Practice Questions | Beginner Level

1. Verify your current working directory?
    ```bash
    pwd
    ```

2. List **/etc** directory files and directories
    ```bash
    ls /etc
    ```

3. List **.conf** files only under **/etc** directory
    ```bash
    ls /etc | grep .conf
    ```
    or
    ```bash
    ls -l /etc/*.conf
    ```

4. Print total number of **.conf** files only under **/etc** directory
    ```bash
    ls -l /etc/*.conf | wc -l
    ```

5. Create an empty directory with name **autopilot** under **/tmp** directory
    ```bash
    mkdir /tmp/autopilot
    ```

6. Create an empty file with name **devops.txt** under **/tmp/autopilot**directory
    ```bash
    touch /tmp/autopilot/devops.txt
    ```

7. Switch your directoy to **/tmp/autopilot/**
    ```bash
    cd /tmp/autopilot/
    ```

8. Switch your directory to **/tmp/autopilot/** and then print "_Hello Devops_" into the **devops.txt** file in the **/tmp/autopilot/** directory
    ```bash
    cd /tmp/autopilot/
    echo "Hello Devops" >> devops.txt
    ```

9. Display the content of **/tmp/autopilot/devops.txt** file on screen
    ```bash
    cat /tmp/autopilot/devops.txt
    ```

10. Switch your directory to **/tmp/autopilot** then create a copy of **devops.txt** file and name the copy as **pilot.txt**
    ```bash
    cd /tmp/autopilot/
    cp devops.txt pilot.txt
    ```

11. Move **/tmp/autopilot/pilot.txt** file to **/etc** directory
    ```bash
    mv /tmp/autopilot/pilot.txt /etc
    ```

12. Delete the file **/etc/pilot.txt**
    ```bash
    rm /etc/pilot.txt
    ```

13. Create an empty file **devops.txt** under **/tmp/autopilot** directory and then remove the file **/tmp/autopilot/devios.txt** forcefully with **rm** command
    ```bash
    touch /tmp/autopilot/devops.txt
    rm -f /tmp/autopilot/devops.txt
    ```

14. Switch your directory to **/etc** and then display top 10 rows of **group** file
    ```bash
    cd /etc/
    head group
    ```

15. Switch your directory to **/etc** and then display top 5 rows of **group** file
    ```bash
    cd /etc/
    head -5 group
    ```

16. Switch your directory to **/etc** and then display last 10 rows of **group** file
    ```bash
    cd /etc/
    tail group
    ```

17. Switch your directory to **/etc** and then display last 2 rows of **group** file
    ```bash
    cd /etc/
    tail -2 group
    ```

18. Print the current date and time on screen
    ```bash
    date
    ```

19. Print the current date in the format **DD/MM/YYYY**
    ```bash
    date "+%d/%m/%Y"
    ```

20. Print the current time in format **HH:MM**
    ```bash
    date "+%H:%M"
    ```

21. Print the current month calender on screen
    ```bash
    cal
    ```

22. Display the hostname of your current server
    ```bash
    hostname
    ```

23. Display the current logged in username
    ```bash
    whoami
    ```

24. ping **udemy.com** from your terminal
    ```bash
    ping udemy.com
    ```

25. Print recently triggered commands on your linux system
    ```bash
    history
    ```
