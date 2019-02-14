# Network Watchdog

A simple network watchdog.

It will visit $HOST every minutes.
If failed, retry; if failed with $MAX_RETRY, do *something*.

Feel free to modify the script.

## Installation

Run below in your terminal:

```bash
git clone https://github.com/QwertyJack/network-watchdog.git && cd network-watchdog
crontab -l | { cat; echo "* * * * * `pwd`/network-watchdog"; } | crontab -
```

Tested under linux.
