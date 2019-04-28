# cle
Command Line Essentials
## [ctop](https://github.com/bcicen/ctop) - top-like interface for docker container
```
ctop -a
```
---
## curl
### Receive public IP address
```
curl ifconfig.me/ip
```
---
## docker
### Build image from Dockerfile with tagging
```
docker build -f Dockerfile -t flow1985/openttd-jgr .
```
### Run command inside container
```
docker exec -it b9edef51a553 /bin/bash
```
---
## git
### TBF
---
## history
### Grep a certain command from history
```
history | grep docker
```
---
## homebrew
### TBF
---
## python
### Serve current directory tree at http://$hostname:8000
```
python -m SimpleHTTPServer
```
## sed - stream editor
### Search and replace text inside a file
### Remove specific line from file specified by line number
```
sed -i '76d' src/rev.cpp.in
```
---
## sox - audio interface
### TBF
---
## sudo - 
### Execute previous command with sudo
```
sudo !!
```
---
## tmux - terminal multiplexer
### Create new session
```
tmux
tmux new
```
### Resume old session (attach)
```
tmux a
```
### Close current session (detach)
```
Prefix + d
``` 




