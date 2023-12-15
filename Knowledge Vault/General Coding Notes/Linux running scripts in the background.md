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

- Check running nohup scripts
```
ps aux | grep notify
```
	The "notify" is part of the scripts name i.e. notify_branch_change.sh 




- ChartEasy
```
nohup ./notify_branch_chart_change.sh > /dev/null 2>&1 &
```