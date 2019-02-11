# downloads-cleanup

This repo will remove files within the specified directory that have been modified more than 7 days ago.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See schedule cleanup for notes on how to execute this script on a set schedule for MacOS.

### Installing

A step by step series of examples that tell you how to execute the cleanup script

Clone repo
```
git clone https://github.com/vinniemo90/downloads-cleanup
```
Execute script
```
python downloads_cleanup.py
```

## Schedule Cleanup

To schedule the cleanup script to run on a mac, follow the below instructions.

1. Modify the plist file (add path to cleanup script and update schedule)
2. Copy plist file to ~/Library/LaunchAgents/
3. Load and start agent using launchctl
```
launchctl load ~/Library/LaunchAgents/solutions.tg4.downloads-cleanup.plist
launchctl start solutions.tg4.downloads-cleanup
```

### More About MacOS Scheduling

https://killtheyak.com/schedule-jobs-launchd/


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
