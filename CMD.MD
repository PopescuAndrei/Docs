#### CMD and Terminal Commands

#### Windows CMD
===

Find and kill processes registered on 8080 port
> for /f "tokens=5" %a in ('netstat -aon ^| find "8080"') do taskkill /f /pid %a


#### Linux Terminal
===

