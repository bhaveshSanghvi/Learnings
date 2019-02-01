# Learnings


## 1. To kill a process which is occupying a port

Step 1: Find the process ID (PID) for the port (e.g.: 8080)

On Windows:
netstat -ao | find "8080"

Other Platforms other than windows :
lsof -i:8080

Step 2: Kill the process ID you found (e.g.: 20712)

On Windows:
Taskkill /PID  20712 /F

Other Platforms other than windows :
kill -9 20712   or kill 20712
