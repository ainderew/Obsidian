Server 

- Give Access
```
chmod +x /path/to/your/script.sh
```

- Run in background
```
nohup ./notify_branch_change.sh > /dev/null 2>&1 &
```

- Kill script
```
pkill -f notify_branch_change.sh
```

- Confirm if running
```
ps aux | grep notify_branch_change.sh
```

