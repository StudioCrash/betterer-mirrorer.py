# mirrorer.py
This is an rsync style python script to mirror the contents of one directory to another, while ignoring DS_Store, spotlight, and trash.

It will prompt user for source and destination in interactive mode, but if supplied arguments, the first argument will be interpreted as the source after a space the second argument will be interpreted as the destination.

It accepts command-line options like:
    1. source
    2. destination
    3. --excludee
    4. --dry-run

If command line arguments are left out, it will use an interactive mode, which prompts the user for the options.

On it's own it doesn't log it's actions, but you can append the following to make it do so:
| tee "logs/sync_script_log_$(date +%Y-%m-%d_%H-%M-%S).log"


