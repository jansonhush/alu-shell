# Processes and Signals

Bash scripts I wrote to practice working with processes and signals.

## What's in here

- `0-what-is-my-pid`: prints the script's own PID
- `1-list_your_processes`: lists all running processes
- `2-show_your_bash_pid`: shows the lines with "bash" in the process list
- `3-show_your_bash_pid_made_easy`: shows the PID and name of bash processes
- `4-to_infinity_and_beyond`: prints "To infinity and beyond" forever
- `5-dont_stop_me_now`: stops script 4 using kill
- `6-stop_me_if_you_can`: stops script 4 without kill or killall
- `7-highlander`: like script 4, but says "I am invincible!!!" when it gets SIGTERM
- `67-stop_me_if_you_can`: sends SIGTERM to 7-highlander
- `8-beheaded_process`: kills 7-highlander for good
- `10-process_and_pid_file`: writes its PID to a file and handles SIGTERM, SIGINT and SIGQUIT
- `manage_my_process`: writes "I am alive!" to /tmp/my_process every 2 seconds
- `11-manage_my_process`: init script to start, stop or restart manage_my_process

## How to run

Make the script executable, then run it:

    chmod u+x 0-what-is-my-pid
    ./0-what-is-my-pid

For the init script, pass start, stop or restart:

    ./11-manage_my_process start
