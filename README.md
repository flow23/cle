# cle
Command Line Essentials
## convert
### Create animated gif from multiple images and loop forever
```
convert -loop 0 -delay 200 1.png 2.png 3.png 4.png 5.png 6.png 7.png 8.png output.gif
```
---
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
### Merge all *.mp3 after one another into one single .mp3 file while using bitrate 192kb/s 
```
sox 0*.mp3 -C 192.01 -c 2 -S "Benjamin Blümchen - 026 - Als Bademeister.mp3"
```
---
## sudo - 
### Execute previous command with sudo
```
sudo !!
```
---
## tar with gzip - tape archiver :) and gunzip
### Create .tar.gz with highest compression
```
env GZIP=-9 tar cvzf file.tar.gz /path/to/directory
```
### List the content of a .tar.gz file
```
tar -ztvf file.tar.gz
```
## tmux - terminal multiplexer
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




